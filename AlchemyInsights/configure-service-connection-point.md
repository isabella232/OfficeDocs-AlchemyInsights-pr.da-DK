---
title: Konfigurere serviceforbindelsespunkt (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035449"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="421f6-102">Konfigurere serviceforbindelsespunkt (SCP)</span><span class="sxs-lookup"><span data-stu-id="421f6-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="421f6-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="421f6-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="421f6-104">**Årsag:** Det er ikke muligt at læse SCP-objektet og hente Azure AD-lejeroplysningerne</span><span class="sxs-lookup"><span data-stu-id="421f6-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="421f6-105">**Løsning:** Se afsnittet Konfigurer [et tjenesteforbindelsespunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="421f6-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="421f6-106">**Handlingsplan**</span><span class="sxs-lookup"><span data-stu-id="421f6-106">**Action plan**</span></span>

- <span data-ttu-id="421f6-107">Kontrollér, om enheden har modtaget gruppepolitikobjektet for den kontrollerede validering.</span><span class="sxs-lookup"><span data-stu-id="421f6-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="421f6-108">Kontrollér, at gruppepolitikobjektet har oprettet registreringsdatabasenøglerne.</span><span class="sxs-lookup"><span data-stu-id="421f6-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="421f6-109">Sørg for, at du har to nøgler oprettet med dit mappe-id og dit onmicrosoft-domæne.</span><span class="sxs-lookup"><span data-stu-id="421f6-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="421f6-110">**Konfigurer indstilling for registreringsdatabase på klientsiden for SCP**</span><span class="sxs-lookup"><span data-stu-id="421f6-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="421f6-111">Brug følgende eksempel til at oprette et Gruppepolitik-objekt (GPO) til at installere en indstilling i registreringsdatabasen, der konfigurerer en SCP-post i registreringsdatabasen på dine enheder.</span><span class="sxs-lookup"><span data-stu-id="421f6-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="421f6-112">Åbn en Gruppepolitik administrationskonsol, og opret et nyt gruppepolitikobjekt i dit domæne.</span><span class="sxs-lookup"><span data-stu-id="421f6-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="421f6-113">Giv dit nyoprettede gruppepolitikobjekt et navn (f.eks. ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="421f6-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="421f6-114">Rediger gruppepolitikobjektet, og find følgende sti: Computerkonfiguration > **Indstillinger > Windows-indstillinger > registreringsdatabase.**</span><span class="sxs-lookup"><span data-stu-id="421f6-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="421f6-115">Højreklik på **registreringsdatabasen, og** vælg **Ny > registreringsdatabaseelement.**</span><span class="sxs-lookup"><span data-stu-id="421f6-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="421f6-116">Konfigurer **følgende** under fanen Generelt:</span><span class="sxs-lookup"><span data-stu-id="421f6-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="421f6-117">**Handling:** Opdater</span><span class="sxs-lookup"><span data-stu-id="421f6-117">**Action**: Update</span></span>
    
- <span data-ttu-id="421f6-118">**Hive:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="421f6-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="421f6-119">**Nøglesti:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="421f6-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="421f6-120">**Værdinavn:** TenantId</span><span class="sxs-lookup"><span data-stu-id="421f6-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="421f6-121">**Værditype:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="421f6-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="421f6-122">**Værdidata:** GUID'et eller mappe-id'et for din Azure AD-forekomst (denne værdi kan findes i **Azure-portalen > Azure Active Directory > Properties > Directory-id)**</span><span class="sxs-lookup"><span data-stu-id="421f6-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="421f6-123">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="421f6-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="421f6-124">Højreklik på **registreringsdatabasen, og** vælg **Ny > registreringsdatabaseelement.**</span><span class="sxs-lookup"><span data-stu-id="421f6-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="421f6-125">Konfigurer **følgende** under fanen Generelt:</span><span class="sxs-lookup"><span data-stu-id="421f6-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="421f6-126">**Handling:** Opdater</span><span class="sxs-lookup"><span data-stu-id="421f6-126">**Action**: Update</span></span>
    
- <span data-ttu-id="421f6-127">**Hive:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="421f6-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="421f6-128">**Nøglesti:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="421f6-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="421f6-129">**Værdinavn:** TenantName</span><span class="sxs-lookup"><span data-stu-id="421f6-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="421f6-130">**Værditype:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="421f6-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="421f6-131">**Værdidata:** Dit bekræftede domænenavn, hvis du bruger et miljø i organisationsnetværket, f.eks. AD FS.</span><span class="sxs-lookup"><span data-stu-id="421f6-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="421f6-132">Dit bekræftede domænenavn eller dit onmicrosoft.com (f.eks. contoso.onmicrosoft).com, hvis du bruger administreret miljø</span><span class="sxs-lookup"><span data-stu-id="421f6-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="421f6-133">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="421f6-133">Click **OK**.</span></span>

7. <span data-ttu-id="421f6-134">Luk editoren for det nyoprettede gruppepolitikobjekt.</span><span class="sxs-lookup"><span data-stu-id="421f6-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="421f6-135">Sammenkæd det nyoprettede gruppepolitikobjekt med de ønskede OU'er, der indeholder domænetilføjede computere, som tilhører din kontrollerede implementerings population.</span><span class="sxs-lookup"><span data-stu-id="421f6-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="421f6-136">Du kan finde flere oplysninger under [Kontrolleret validering af hybrid Azure AD-joinforbindelse – Azure AD | Microsoft Docs og](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) fejlfinding [af hybridenheder, der er forbundet til Azure Active Directory, | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)</span><span class="sxs-lookup"><span data-stu-id="421f6-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









