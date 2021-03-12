---
title: Office kan ikke aktiveres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704924"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="dd23c-102">Office kan ikke aktiveres</span><span class="sxs-lookup"><span data-stu-id="dd23c-102">Unable to activate Office</span></span>

- <span data-ttu-id="dd23c-103">Kontrollér, om din abonnementsstatus er udløbet.</span><span class="sxs-lookup"><span data-stu-id="dd23c-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="dd23c-104">Sørg for, at du har et abonnement, der tillader klientlicenser, f.eks Office 365 Business eller Business Premium, og sørg for, at brugeren [har fået tildelt en licens.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="dd23c-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="dd23c-105">Sørg for, at brugeren logger på Office med den samme konto som den, der har fået licensen tildelt.</span><span class="sxs-lookup"><span data-stu-id="dd23c-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="dd23c-106">Se [siden Tjenestetilstand for Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) for at finde ud af, om der er nogen kendte problemer med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="dd23c-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="dd23c-107">Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer adgangen til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="dd23c-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="dd23c-108">Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL-adresser og IP-adresseintervaller").</span><span class="sxs-lookup"><span data-stu-id="dd23c-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="dd23c-109">**Tip** På Windows-computere kan vi diagnosticere og automatisk løse flere almindelige office-logonproblemer for dig.</span><span class="sxs-lookup"><span data-stu-id="dd23c-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="dd23c-110">Download og kør  **[Microsoft Support- og genoprettelsesassistent for](https://aka.ms/SaRA-OfficeSignInScenario)** at bruge vores automatiserede værktøj.</span><span class="sxs-lookup"><span data-stu-id="dd23c-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="dd23c-111">Brug følgende fejlfindingshandlinger:</span><span class="sxs-lookup"><span data-stu-id="dd23c-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="dd23c-112">Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="dd23c-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="dd23c-113">[Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tildel](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen igen, og [log på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="dd23c-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="dd23c-114">Brug [Fejlfindingsværktøj til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="dd23c-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="dd23c-115">Nulstil aktiveringstilstand for Office</span><span class="sxs-lookup"><span data-stu-id="dd23c-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nulstil Office-aktiveringstilstanden")
- [<span data-ttu-id="dd23c-116">Udfør en onlinereparation af Office</span><span class="sxs-lookup"><span data-stu-id="dd23c-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="dd23c-117">Hvis du vil have yderligere fejlfindingsløsninger, skal du se:</span><span class="sxs-lookup"><span data-stu-id="dd23c-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="dd23c-118">Fejl i forbindelse med produkt uden licens og aktivering i Office</span><span class="sxs-lookup"><span data-stu-id="dd23c-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="dd23c-119">"Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office</span><span class="sxs-lookup"><span data-stu-id="dd23c-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)