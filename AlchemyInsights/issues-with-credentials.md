---
title: Problemer med legitimationsoplysninger
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063600"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="915a3-102">Problemer med legitimationsoplysninger</span><span class="sxs-lookup"><span data-stu-id="915a3-102">Issues with credentials</span></span>

<span data-ttu-id="915a3-103">Microsoft-identitetsplatformen og flowet til klientlegitimationsoplysninger for [OAuth 2.0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver, hvordan du programmerer direkte mod tildelingsflowet for OAuth 2.0-klientlegitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="915a3-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="915a3-104">**Hvordan administrerer jeg et programs adgangskode eller legitimationsoplysninger til certifikater?**</span><span class="sxs-lookup"><span data-stu-id="915a3-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="915a3-105">I Azure CLI kan du bruge [az ad app-legitimationsoplysninger](https://docs.microsoft.com/cli/azure/ad/app/credential) til at slette, angive eller nulstille et apps adgangskode- eller certifikatlegitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="915a3-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="915a3-106">**Hvordan nulstiller mine brugere deres adgangskoder?**</span><span class="sxs-lookup"><span data-stu-id="915a3-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="915a3-107">Brugerne skal registrere [sig til selvbetjening for nulstilling af adgangskode,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) før de kan nulstille deres adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="915a3-108">Når en bruger er registreret, kan brugeren følge instruktionerne i denne artikel for at nulstille sin adgangskode: [Nulstil din arbejds- eller skoleadgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="915a3-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="915a3-109">**Hvordan ændrer mine brugere deres adgangskoder?**</span><span class="sxs-lookup"><span data-stu-id="915a3-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="915a3-110">Brugerne kan følge trinnene i denne artikel for at ændre deres adgangskoder: [Sådan ændrer du din adgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="915a3-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="915a3-111">De kan også [administrere appadgangskoder for totrinsbekræftelse.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="915a3-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="915a3-112">**Min bruger får en fejl, når han eller hun ændrer eller nulstiller sin adgangskode**</span><span class="sxs-lookup"><span data-stu-id="915a3-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="915a3-113">Dette link indeholder oplysninger om almindelige problemer, der kan opstå, når en bruger forsøger at nulstille sin adgangskode: [almindelige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="915a3-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="915a3-114">**Jeg har problemer med at nulstille en brugers adgangskode**</span><span class="sxs-lookup"><span data-stu-id="915a3-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="915a3-115">Sørg for, at du har tilladelse til at nulstille adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="915a3-116">*Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.*</span><span class="sxs-lookup"><span data-stu-id="915a3-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="915a3-117">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="915a3-118">Sørg for, at du forstår licenskravene:</span><span class="sxs-lookup"><span data-stu-id="915a3-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="915a3-119">Du skal have mindst én licens tildelt i organisationen:</span><span class="sxs-lookup"><span data-stu-id="915a3-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="915a3-120">**Kun brugere i skyen** – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="915a3-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="915a3-121">**Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="915a3-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="915a3-122">Du kan få mere at vide om licenskrav under Licenskrav til nulstilling af adgangskode [til Azure AD via selvbetjening.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="915a3-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="915a3-123">Hvis du vil nulstille en brugers adgangskode, skal du finde brugeren i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="915a3-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="915a3-124">Klik derefter på knappen "Nulstil adgangskode" på oversigtsbladet for den pågældende bruger.</span><span class="sxs-lookup"><span data-stu-id="915a3-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="915a3-125">**Knappen til nulstilling af adgangskode er nedtonet**</span><span class="sxs-lookup"><span data-stu-id="915a3-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="915a3-126">Du er ikke autoriseret til **at nulstille** denne brugers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="915a3-127">*Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.*</span><span class="sxs-lookup"><span data-stu-id="915a3-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="915a3-128">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="915a3-129">**Jeg kan ikke se bladet til nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="915a3-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="915a3-130">Du er ikke autoriseret til at nulstille adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="915a3-131">*Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.*</span><span class="sxs-lookup"><span data-stu-id="915a3-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="915a3-132">Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="915a3-133">**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="915a3-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="915a3-134">Integrations bladet i det lokale miljø vises kun i hybridmiljøer – dvs. at du bruger tilbageførsel af adgangskode til at manipulere lokale brugeres adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="915a3-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="915a3-135">Du kan ikke se denne blade, hvis:</span><span class="sxs-lookup"><span data-stu-id="915a3-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="915a3-136">Du bruger ikke tilbageførsel af adgangskode</span><span class="sxs-lookup"><span data-stu-id="915a3-136">You are not using password writeback</span></span>
  - <span data-ttu-id="915a3-137">Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode</span><span class="sxs-lookup"><span data-stu-id="915a3-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="915a3-138">Der er et problem med din installation/forbindelse til Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="915a3-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="915a3-139">Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode under [Fejlfinding af tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="915a3-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="915a3-140">**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**</span><span class="sxs-lookup"><span data-stu-id="915a3-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="915a3-141">Log på Azure-portalen som en relevant administrator.</span><span class="sxs-lookup"><span data-stu-id="915a3-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="915a3-142">Gå til siden **Brugere og grupper,** og vælg **Alle brugere.**</span><span class="sxs-lookup"><span data-stu-id="915a3-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="915a3-143">Vælg en bruger på listen.</span><span class="sxs-lookup"><span data-stu-id="915a3-143">Select a user from the list.</span></span>
4. <span data-ttu-id="915a3-144">Vælg Oversigt for den valgte **bruger,** og vælg derefter Nulstil adgangskode på **kommandolinjen.**</span><span class="sxs-lookup"><span data-stu-id="915a3-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="915a3-145">Vælg knappen **Nulstil** adgangskode, og følg vejledningen på skærmen.</span><span class="sxs-lookup"><span data-stu-id="915a3-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="915a3-146">Kun nulstillinger, der udføres via **Azure-portalen, understøtter** tilbageførsel af adgangskode.</span><span class="sxs-lookup"><span data-stu-id="915a3-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="915a3-147">**Jeg nulstiller en lokal brugers adgangskode fra Office 365-administrationsportalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**</span><span class="sxs-lookup"><span data-stu-id="915a3-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="915a3-148">Tilbageførsel af adgangskode understøttes ikke i denne portal.</span><span class="sxs-lookup"><span data-stu-id="915a3-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="915a3-149">Nulstil brugerens adgangskode igen i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="915a3-149">Reset the user's password again in the Azure portal.</span></span>
