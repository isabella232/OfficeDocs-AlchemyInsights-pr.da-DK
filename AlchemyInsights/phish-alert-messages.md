---
title: 2491 Alert e-mails fra 'Phish Leveret på grund af lejer eller bruger tilsidesætte'-politik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758902"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f2e8f-102">Giv e-mails besked fra politikken "Phish Delivered due to tenant or user override"</span><span class="sxs-lookup"><span data-stu-id="f2e8f-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f2e8f-103">En standardadvarselspolitik med navnet "Phish Delivered due to tenant or user override" er blevet udrullet til lejere med Office 365 ATP P1- og P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="f2e8f-104">Hvis du har modtaget denne besked, er her trinnene til at undersøge:</span><span class="sxs-lookup"><span data-stu-id="f2e8f-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f2e8f-105">Klik på Vis **besked** i beskedbeskeden for at gå til siden **Beskeder** i Sikkerheds& Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f2e8f-106">Vælg beskeden for at få vist indstillingen **Vis meddelelsesliste** eller **Vis meddelelser i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f2e8f-107">Begge disse indstillinger tager dig til detaljerne i meddelelsen, som omfatter meddelelses-id'et.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f2e8f-108">Bemærk, at linket Trusselsfinder automatisk filtrerer de meddelelser, der opfylder advarselskriterierne.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f2e8f-109">Du skal muligvis justere datofilteret i Trusselstifinder.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f2e8f-110">Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:</span><span class="sxs-lookup"><span data-stu-id="f2e8f-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f2e8f-111">En tilladt afsender eller et tilladt domæne, der er angivet af brugeren.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f2e8f-112">En tilladt afsender eller et tilladt domæne, der er indstillet af administratoren i en antispampolitik.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f2e8f-113">En tilladt IP-adresse i en politik for forbindelsesfilter.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f2e8f-114">En mailflowregel (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f2e8f-115">Hvis du mener, at meddelelsen er markeret forkert som phish, skal du bruge [tilføjelsesprogrammet Outlook-rapportmeddelelse](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til at sende meddelelseseksempler til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2e8f-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
