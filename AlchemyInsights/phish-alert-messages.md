---
title: 2491 Giv mails besked fra politikken "Phish leveret på grund af lejer eller brugertilsidesættelse"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544572"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="b4488-102">Giv besked om mails fra politikken "Phish leveret på grund af lejer eller brugertilsidesættelse"</span><span class="sxs-lookup"><span data-stu-id="b4488-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="b4488-103">En standardbeskedpolitik med navnet "Phish Leveret pga. lejer eller brugertilsidesættelse" er blevet udrullet til lejere med Microsoft Defender Office 365 P1- og P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="b4488-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="b4488-104">Hvis du har modtaget denne besked, skal du undersøge følgende:</span><span class="sxs-lookup"><span data-stu-id="b4488-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="b4488-105">I beskeden skal du klikke på **Vis besked** for at gå til **siden** Vigtige beskeder i & Security Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="b4488-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="b4488-106">Vælg beskeden for at få vist indstillingen Vis **meddelelsesliste eller** **Vis meddelelser i Stifinder.**</span><span class="sxs-lookup"><span data-stu-id="b4488-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="b4488-107">Begge disse indstillinger giver dig adgang til detaljerne i meddelelsen, som indeholder meddelelses-id'et.</span><span class="sxs-lookup"><span data-stu-id="b4488-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="b4488-108">Bemærk, at linket Threat Explorer automatisk filtrerer de meddelelser, der opfylder beskedkriterierne.</span><span class="sxs-lookup"><span data-stu-id="b4488-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="b4488-109">Du skal muligvis justere datofilteret i Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="b4488-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="b4488-110">Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:</span><span class="sxs-lookup"><span data-stu-id="b4488-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="b4488-111">En tilladt afsender eller et domæne, der er angivet af brugeren.</span><span class="sxs-lookup"><span data-stu-id="b4488-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="b4488-112">En tilladt afsender eller et domæne, der er angivet af administratoren i en politik for uønsket post.</span><span class="sxs-lookup"><span data-stu-id="b4488-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="b4488-113">En tilladt IP-adresse i en forbindelsesfilterpolitik.</span><span class="sxs-lookup"><span data-stu-id="b4488-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="b4488-114">En regel for mailflow (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.</span><span class="sxs-lookup"><span data-stu-id="b4488-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="b4488-115">Hvis du mener, at meddelelsen er forkert markeret som [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) phish, skal du bruge tilføjelsesprogrammet Rapportmeddelelse Outlook at sende meddelelseseksempler til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b4488-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
