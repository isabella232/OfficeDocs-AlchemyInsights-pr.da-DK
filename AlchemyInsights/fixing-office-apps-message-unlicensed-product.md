---
title: Det er ikke muligt at Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798674"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="f86aa-102">Det er ikke muligt at Office</span><span class="sxs-lookup"><span data-stu-id="f86aa-102">Unable to activate Office</span></span>

<span data-ttu-id="f86aa-103">**Bemærk!** Hvis du bruger en ældre version af Windows (f.eks. Windows 7), skal du sørge for, at TLS 1.2 er aktiveret som standard.</span><span class="sxs-lookup"><span data-stu-id="f86aa-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="f86aa-104">Få mere at vide under Opdater for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .</span><span class="sxs-lookup"><span data-stu-id="f86aa-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="f86aa-105">Kontrollér, om din abonnementsstatus er udløbet.</span><span class="sxs-lookup"><span data-stu-id="f86aa-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="f86aa-106">Sørg for, at du har et abonnement, der tillader klientlicenser, f.eks. Office 365 Business eller Business Premium, og sørg for, at [brugeren har fået tildelt en licens.](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="f86aa-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="f86aa-107">Sørg for, at brugeren logger på Office med den samme konto som den, der har fået licensen tildelt.</span><span class="sxs-lookup"><span data-stu-id="f86aa-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="f86aa-108">Se [siden Tjenestetilstand for Office 365](/office365/enterprise/view-service-health) for at finde ud af, om der er nogen kendte problemer med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f86aa-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="f86aa-109">Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke Microsoft 365 adgang til internettet.</span><span class="sxs-lookup"><span data-stu-id="f86aa-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="f86aa-110">Se [URL-adresser og IP-adresseområder for Office 365](/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL-adresser og IP-adresseintervaller").</span><span class="sxs-lookup"><span data-stu-id="f86aa-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="f86aa-111">**Tip** På Windows computere kan vi diagnosticere og automatisk løse forskellige almindelige Office problemer med logon for dig.</span><span class="sxs-lookup"><span data-stu-id="f86aa-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="f86aa-112">Download og kør **[Microsoft-Support- og genoprettelsesassistent](https://aka.ms/SaRA-OfficeSignInScenario)** at bruge vores automatiserede værktøj.</span><span class="sxs-lookup"><span data-stu-id="f86aa-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="f86aa-113">Brug følgende fejlfindingshandlinger:</span><span class="sxs-lookup"><span data-stu-id="f86aa-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="f86aa-114">Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="f86aa-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="f86aa-115">[Fjern](/microsoft-365/admin/manage/remove-licenses-from-users) og [Tildel](/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen igen, og [log på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="f86aa-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="f86aa-116">Brug [Fejlfindingsværktøj til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="f86aa-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="f86aa-117">Nulstil aktiveringstilstand for Office</span><span class="sxs-lookup"><span data-stu-id="f86aa-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nulstil Office aktiveringstilstand")
- [<span data-ttu-id="f86aa-118">Udfør en onlinereparation af Office</span><span class="sxs-lookup"><span data-stu-id="f86aa-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="f86aa-119">Hvis du vil have yderligere fejlfindingsløsninger, skal du se:</span><span class="sxs-lookup"><span data-stu-id="f86aa-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="f86aa-120">Fejl i forbindelse med produkt uden licens og aktivering i Office</span><span class="sxs-lookup"><span data-stu-id="f86aa-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="f86aa-121">"Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office</span><span class="sxs-lookup"><span data-stu-id="f86aa-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)