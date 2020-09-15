---
title: 1385 – Office-365-Alert-Policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664020"
---
# <a name="alert-policies"></a><span data-ttu-id="2a45b-102">Påmindelses politikker</span><span class="sxs-lookup"><span data-stu-id="2a45b-102">Alert policies</span></span>

<span data-ttu-id="2a45b-103">Microsoft 365 Security & overholdelses Center indeholder [standard påmindelses politikker](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) , der udløser beskeder for organisationer med et Office 365 Enterprise-eller Office 365 amerikanske--, E3/G3-eller E5/G5-abonnement.</span><span class="sxs-lookup"><span data-stu-id="2a45b-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="2a45b-104">Derfor modtager administratorerne en meddelelse om en advarsel via mail, der sendes af Office365Alerts@microsoft.com med en emnelinje, f. eks "en lav prioritet: *navnet på besked politikken*".</span><span class="sxs-lookup"><span data-stu-id="2a45b-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="2a45b-105">Påmindelser sendes, når der udløses påmindelser for almindelige aktiviteter, f. eks når brugere:</span><span class="sxs-lookup"><span data-stu-id="2a45b-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="2a45b-106">Opret indbakkeregler, der videresender mail.</span><span class="sxs-lookup"><span data-stu-id="2a45b-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="2a45b-107">Tildel tilladelser til deres postkasse.</span><span class="sxs-lookup"><span data-stu-id="2a45b-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="2a45b-108">Del eller slet et stort antal filer i SharePoint-fildeling.</span><span class="sxs-lookup"><span data-stu-id="2a45b-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="2a45b-109">Opret eDiscovery-søgninger, og eksportér søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="2a45b-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="2a45b-110">Sådan gennemser og reagerer en besked:</span><span class="sxs-lookup"><span data-stu-id="2a45b-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="2a45b-111">Gå til [Security & Overholdelsescenter](https://protection.office.com) , og log på.</span><span class="sxs-lookup"><span data-stu-id="2a45b-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="2a45b-112">Klik på **beskeder**  >  **Vis beskeder**.</span><span class="sxs-lookup"><span data-stu-id="2a45b-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="2a45b-113">Klik på en besked for at få vist en pop op-side med oplysninger om beskeden.</span><span class="sxs-lookup"><span data-stu-id="2a45b-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="2a45b-114">Du kan reagere på en besked, f. eks at [fjerne en mistænkelig indbakke regel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="2a45b-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="2a45b-115">Du kan også lukke beskeden ved at klikke på **løs** på pop op-siden med advarslen.</span><span class="sxs-lookup"><span data-stu-id="2a45b-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="2a45b-116">Du kan finde flere oplysninger om, hvordan du konfigurerer og administrerer påmindelses politikker, i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="2a45b-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="2a45b-117">**Vigtigt**! besked om påmindelse via mail fra Microsoft vil aldrig bede dig om at gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="2a45b-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="2a45b-118">Angive en adgangskode</span><span class="sxs-lookup"><span data-stu-id="2a45b-118">Provide a password</span></span>
- <span data-ttu-id="2a45b-119">Bekræft sikkerheds detaljerne for din konto</span><span class="sxs-lookup"><span data-stu-id="2a45b-119">Verify the security details of your account</span></span>
- <span data-ttu-id="2a45b-120">Godkend dig selv igen</span><span class="sxs-lookup"><span data-stu-id="2a45b-120">Re-authenticate yourself</span></span>

<span data-ttu-id="2a45b-121">Hvis du modtager en mail som denne, blev den ikke sendt af Microsoft, og det anses for at være en phishing-bedrageri.</span><span class="sxs-lookup"><span data-stu-id="2a45b-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="2a45b-122">Hvis det sker, skal du [rapportere det til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="2a45b-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>