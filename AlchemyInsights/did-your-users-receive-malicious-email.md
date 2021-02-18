---
title: Modtog dine brugere skadelig mail
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291786"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="4a616-102">Modtog dine brugere skadelige mails?</span><span class="sxs-lookup"><span data-stu-id="4a616-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="4a616-103">Du kan nu rapportere den skadelige mail til Microsoft ved hjælp af [administrationsindsendelser i Security & Compliance Center.](https://sip.protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="4a616-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="4a616-104">Meddelelser, der er sendt [i administratorindsendelser, scannes,](https://sip.protection.office.com/reportsubmission) og følgende resultater vises i pop **op-pop op-mailen** med oplysninger:</span><span class="sxs-lookup"><span data-stu-id="4a616-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="4a616-105">Hvis der opstod en fejl i afsenderens mailgodkendelse på leveringstidspunktet.</span><span class="sxs-lookup"><span data-stu-id="4a616-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="4a616-106">Oplysninger om eventuelle politikhits, der kan have påvirket eller tilsidesat konklusionen i en meddelelse.</span><span class="sxs-lookup"><span data-stu-id="4a616-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="4a616-107">Aktuelle detonationsresultater for at se, om URL-adresserne eller filerne i meddelelsen var skadelige eller ej.</span><span class="sxs-lookup"><span data-stu-id="4a616-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="4a616-108">Feedback fra gradere</span><span class="sxs-lookup"><span data-stu-id="4a616-108">Feedback from graders</span></span>

<span data-ttu-id="4a616-109">Hvis der blev fundet en tilsidesættelse, bør genscanning fuldføres på flere minutter.</span><span class="sxs-lookup"><span data-stu-id="4a616-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="4a616-110">Hvis der ikke var et problem med mailgodkendelse, eller hvis leveringen ikke blev påvirket af en tilsidesættelse, kan det tage op til en dags feedback fra graderne.</span><span class="sxs-lookup"><span data-stu-id="4a616-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="4a616-111">Hvis du er uenig i den endelige vurdering af en meddelelse, URL-adresse eller fil (blokeret vs. ikke blokeret), skal du sende meddelelsen igen efter en dag til gennemscanning.</span><span class="sxs-lookup"><span data-stu-id="4a616-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="4a616-112">Der er stor risiko for, at konklusionen vil blive ændret, når du har sendt meddelelsen igen.</span><span class="sxs-lookup"><span data-stu-id="4a616-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="4a616-113">I mellemtiden kan du fjerne ondsindede mails fra brugernes indbakker ved at følge vejledningen i [denne artikel.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="4a616-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="4a616-114">Kunder med Microsoft Defender til Office 365 kan:</span><span class="sxs-lookup"><span data-stu-id="4a616-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="4a616-115">brug [Trusselsstifinder til at finde og slette mistænkelige mails](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="4a616-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="4a616-116">[Brug sikre links til at blokere adgangen til](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) en skadelig URL-adresse</span><span class="sxs-lookup"><span data-stu-id="4a616-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="4a616-117">Spor brugere, der klikkede på og tilgåede ondsindede URL-adresser: [Få vist phishing-URL-adresse,](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)og klik på  &  [advarselsdataene Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="4a616-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="4a616-118">starte en [automatiseret undersøgelse manuelt](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="4a616-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="4a616-119">Du kan også beskytte dig mod skadelige filer og URL-adresser ved at følge vejledningen i [Beskyttelse mod skadelige URL-adresser og filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)</span><span class="sxs-lookup"><span data-stu-id="4a616-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>