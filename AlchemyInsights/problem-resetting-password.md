---
title: Problem med nulstilling af adgangskode
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693390"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="88a11-102">Problemer med nulstilling af adgangskode</span><span class="sxs-lookup"><span data-stu-id="88a11-102">Problems resetting password</span></span>

<span data-ttu-id="88a11-103">Følgende er nogle af de problemer, du kan komme ud for, når du nulstiller adgangskoden og de mulige løsninger:</span><span class="sxs-lookup"><span data-stu-id="88a11-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="88a11-104">**Jeg har et problem med nulstilling af adgangskode, der ikke er dækket af de andre kategorier**</span><span class="sxs-lookup"><span data-stu-id="88a11-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="88a11-105">Sørg for, at du er godkendt til at nulstille adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="88a11-106">Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="88a11-107">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="88a11-108">Sørg for, at du forstår licenskravene:</span><span class="sxs-lookup"><span data-stu-id="88a11-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="88a11-109">Du skal have mindst én licens tildelt i organisationen</span><span class="sxs-lookup"><span data-stu-id="88a11-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="88a11-110">Kun brugere i skyen – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="88a11-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="88a11-111">Sky- og/eller lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="88a11-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="88a11-112">Du kan læse mere om licenskrav i artiklen [Licenseringskrav til nulstilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)af adgangskode til Azure AD via selvbetjening.</span><span class="sxs-lookup"><span data-stu-id="88a11-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="88a11-113">**Jeg har problemer med at teste den politik for nulstilling af adgangskode, jeg har angivet**</span><span class="sxs-lookup"><span data-stu-id="88a11-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="88a11-114">De senest anvendte politikker kan tage flere minutter at replikere på tværs af alle datacentre og slutpunkter.</span><span class="sxs-lookup"><span data-stu-id="88a11-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="88a11-115">Fysisk afstand fra datacenteret påvirker også, hvor hurtigt ændringerne anvendes.</span><span class="sxs-lookup"><span data-stu-id="88a11-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="88a11-116">Test med en slutbruger, ikke en administrator, og test med et lille sæt af brugere.</span><span class="sxs-lookup"><span data-stu-id="88a11-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="88a11-117">De politikker, der er konfigureret i Azure-portalen, gælder KUN for slutbrugere, ikke administratorer.</span><span class="sxs-lookup"><span data-stu-id="88a11-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="88a11-118">Microsoft har en stærk standardpolitik for nulstilling af adgangskode til to porte for alle Azure-administratorroller (eksempel: Global administrator, Helpdesk-administrator, Adgangskodeadministrator osv.)</span><span class="sxs-lookup"><span data-stu-id="88a11-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="88a11-119">Få mere at vide [om politikker for administratorer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="88a11-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="88a11-120">**Jeg vil installere nulstilling af adgangskode, men jeg vil ikke have mine brugere til at registrere yderligere sikkerhedsoplysninger**</span><span class="sxs-lookup"><span data-stu-id="88a11-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="88a11-121">Forudindstille data for dine brugere, så de ikke behøver at gøre det!</span><span class="sxs-lookup"><span data-stu-id="88a11-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="88a11-122">– Som administrator kan du angive telefon- og mailegenskaber for dine brugere, før du udruller nulstilling af adgangskode til organisationen.</span><span class="sxs-lookup"><span data-stu-id="88a11-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="88a11-123">Du kan gøre dette ved hjælp af en API, PowerShell eller Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="88a11-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="88a11-124">Flere oplysninger her:</span><span class="sxs-lookup"><span data-stu-id="88a11-124">More information here:</span></span>
- [<span data-ttu-id="88a11-125">Installation af nulstilling af adgangskode uden at kræve, at brugerne skal registrere sig</span><span class="sxs-lookup"><span data-stu-id="88a11-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="88a11-126">Hvilke data bruges ved nulstilling af adgangskode</span><span class="sxs-lookup"><span data-stu-id="88a11-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="88a11-127">**Knappen til nulstilling af adgangskode er nedtonet**</span><span class="sxs-lookup"><span data-stu-id="88a11-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="88a11-128">Du er ikke autoriseret til at nulstille denne brugers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="88a11-129">Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="88a11-130">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="88a11-131">**Jeg kan ikke se bladet til nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="88a11-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="88a11-132">Du er ikke autoriseret til at nulstille adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="88a11-133">Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="88a11-134">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="88a11-135">**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="88a11-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="88a11-136">Integrations bladet i det lokale miljø vises kun i hybridmiljøer – dvs. at du bruger tilbageførsel af adgangskode til at manipulere lokale brugeres adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88a11-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="88a11-137">Du kan ikke se denne blade, hvis:</span><span class="sxs-lookup"><span data-stu-id="88a11-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="88a11-138">Du bruger ikke tilbageførsel af adgangskode</span><span class="sxs-lookup"><span data-stu-id="88a11-138">You are not using password writeback</span></span>
    - <span data-ttu-id="88a11-139">Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode</span><span class="sxs-lookup"><span data-stu-id="88a11-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="88a11-140">Der er et problem med din installation/forbindelse til Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="88a11-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="88a11-141">Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode i afsnittet Fejlfinding [af tilbageskrivning af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="88a11-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="88a11-142">**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**</span><span class="sxs-lookup"><span data-stu-id="88a11-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="88a11-143">Log på Azure-portalen som en relevant administrator.</span><span class="sxs-lookup"><span data-stu-id="88a11-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="88a11-144">Gå til siden Brugere og grupper, og vælg **Alle brugere.**</span><span class="sxs-lookup"><span data-stu-id="88a11-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="88a11-145">Vælg en bruger på listen.</span><span class="sxs-lookup"><span data-stu-id="88a11-145">Select a user from the list.</span></span>
1. <span data-ttu-id="88a11-146">Vælg Oversigt for den valgte **bruger,** og klik derefter på Nulstil adgangskode på **kommandolinjen.**</span><span class="sxs-lookup"><span data-stu-id="88a11-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="88a11-147">Følg vejledningen på skærmen.</span><span class="sxs-lookup"><span data-stu-id="88a11-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="88a11-148">Kun nulstillinger, der udføres via Azure-portalen, understøtter tilbageførsel af adgangskode.</span><span class="sxs-lookup"><span data-stu-id="88a11-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="88a11-149">**Jeg nulstiller en lokal brugers adgangskode fra Office 365-administrationsportalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**</span><span class="sxs-lookup"><span data-stu-id="88a11-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="88a11-150">Tilbageførsel af adgangskode understøttes ikke i denne portal.</span><span class="sxs-lookup"><span data-stu-id="88a11-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="88a11-151">Nulstil brugerens adgangskode igen i Azure-portalen – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="88a11-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

