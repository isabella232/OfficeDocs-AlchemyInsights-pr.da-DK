---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533801"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d8284-102">Fejlfinding i forbindelse med synkronisering af adgangskoder</span><span class="sxs-lookup"><span data-stu-id="d8284-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d8284-103">Fejlfinding af problemer, hvor ingen adgangskoder er synkroniseret med Azure AD Connect version 1.1.614.0 eller nyere:</span><span class="sxs-lookup"><span data-stu-id="d8284-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d8284-104">Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren med indstillingen **Kør som Administrator** .</span><span class="sxs-lookup"><span data-stu-id="d8284-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="d8284-105">Køre **Set-Udførselspolitikken RemoteSigned** eller **ubegrænset sæt Udførselspolitikken**.</span><span class="sxs-lookup"><span data-stu-id="d8284-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="d8284-106">Start guiden Opret forbindelse Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8284-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="d8284-107">Gå til siden **Yderligere opgaver** , Vælg **fejlfinding**, og klik på **Næste**.</span><span class="sxs-lookup"><span data-stu-id="d8284-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="d8284-108">Klik på menuen **Start til at starte fejlfindingen** PowerShell på siden fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="d8284-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="d8284-109">I hovedmenuen, Vælg **Fejlfinding i forbindelse med synkronisering af adgangskoder**.</span><span class="sxs-lookup"><span data-stu-id="d8284-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="d8284-110">Vælg i menuen sub **adgangskodesynkronisering virker ikke på alle**.</span><span class="sxs-lookup"><span data-stu-id="d8284-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="d8284-111">**Forstå resultaterne af fejlfinding i forbindelse med opgaven**</span><span class="sxs-lookup"><span data-stu-id="d8284-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d8284-112">Fejlfinding i forbindelse med opgaven udføres følgende kontrol:</span><span class="sxs-lookup"><span data-stu-id="d8284-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d8284-113">Validerer, at funktionen til synkronisering af adgangskode er aktiveret for din Azure AD lejer.</span><span class="sxs-lookup"><span data-stu-id="d8284-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="d8284-114">Validerer, Azure AD Connect-serveren ikke er i midlertidig tilstand.</span><span class="sxs-lookup"><span data-stu-id="d8284-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="d8284-115">For hver eksisterende lokale Active Directory connector (hvilket svarer til en eksisterende Active Directory-skov):</span><span class="sxs-lookup"><span data-stu-id="d8284-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="d8284-116">Validerer, at funktionen til synkronisering af adgangskode er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="d8284-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="d8284-117">Søger efter adgangskode synkronisering heartbeat-hændelser i logfilerne Windows Application Event.</span><span class="sxs-lookup"><span data-stu-id="d8284-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="d8284-118">For hver Active Directory-domæne i det lokale Active Directory connector:</span><span class="sxs-lookup"><span data-stu-id="d8284-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="d8284-119">Validerer, at domænet kan nås fra Azure AD Connect-serveren.</span><span class="sxs-lookup"><span data-stu-id="d8284-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="d8284-120">Validerer, at kontiene Active Directory-domæneservices (AD DS), der bruges af den lokale Active Directory connector har det rigtige brugernavn, adgangskode og tilladelser, der kræves af synkronisering af adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="d8284-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="d8284-121">Du kan finde yderligere hjælp til fejlfinding af synkronisering af adgangskode, [fejlfinding i forbindelse med synkronisering af adgangskoder med Azure Connect for AD-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d8284-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  