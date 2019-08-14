---
title: 2491 e-mail-påmindelser fra politikken 'Phish leveres på grund af lejer eller bruger override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391196"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="2be4a-102">E-mail-påmindelser fra politikken 'Phish leveres på grund af lejer eller bruger override'</span><span class="sxs-lookup"><span data-stu-id="2be4a-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="2be4a-103">En standard besked politik med navnet "Phish leveret på grund af lejer eller bruger override" har ført til lejere med Office 365 DTT P1 og P2 licenser.</span><span class="sxs-lookup"><span data-stu-id="2be4a-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="2be4a-104">Hvis du har modtaget denne besked, er her de skridt til at undersøge:</span><span class="sxs-lookup"><span data-stu-id="2be4a-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="2be4a-105">Fra beskeden, skal du klikke på **Vis besked** for at gå til siden **beskeder** i sikkerhed & Overholdelsescenter.</span><span class="sxs-lookup"><span data-stu-id="2be4a-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="2be4a-106">Marker beskeden, du vil se indstillingen til **visning af meddelelseslisten** eller **få vist meddelelser i Explorer**.</span><span class="sxs-lookup"><span data-stu-id="2be4a-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="2be4a-107">Begge indstillinger kommer du til detaljerne i e-mailen, der indeholder meddelelsen-ID.</span><span class="sxs-lookup"><span data-stu-id="2be4a-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="2be4a-108">Bemærk, at linket trussel Explorer automatisk filtrere meddelelser, der opfylder kriterierne for påmindelser.</span><span class="sxs-lookup"><span data-stu-id="2be4a-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="2be4a-109">Du skal muligvis justere Datofilter i Explorer trussel.</span><span class="sxs-lookup"><span data-stu-id="2be4a-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="2be4a-110">Phishing-meddelelsen blev leveret på grund af en tilsidesættelse af manuelt konfigureret:</span><span class="sxs-lookup"><span data-stu-id="2be4a-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="2be4a-111">En tilladt afsender eller et domæne, der er angivet af brugeren.</span><span class="sxs-lookup"><span data-stu-id="2be4a-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="2be4a-112">En tilladt afsender eller et domæne, der er angivet af administratoren i en politik om uønskede e-mails.</span><span class="sxs-lookup"><span data-stu-id="2be4a-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="2be4a-113">Tilladte IP-adresse i en filter forbindelser.</span><span class="sxs-lookup"><span data-stu-id="2be4a-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="2be4a-114">En mail flow-regel (også kendt som transport), der er konfigureret til at tillade meddelelser i.</span><span class="sxs-lookup"><span data-stu-id="2be4a-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="2be4a-115">Hvis du mener, at meddelelsen blev fejlagtigt markeret som phish, bruge Outlook- [tilføjelsesprogrammet rapporteringsmeddelelse](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) skal forelægge prøver af meddelelsen til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2be4a-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
