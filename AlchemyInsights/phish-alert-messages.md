---
title: 2491 Giv besked via mail fra den ' Phish, der er leveret på grund af politikken for lejer eller bruger tilsidesættelse "
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728605"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="92281-102">Giv mails besked fra politikken "leveret, der er leveret på grund af leje-eller bruger tilsidesættelse"</span><span class="sxs-lookup"><span data-stu-id="92281-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="92281-103">En standard besked politik med navnet "Phish leveret på grund af leje-eller bruger tilsidesættelse" er blevet udrullet til lejere med Office 365 DTT-licenser og P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="92281-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="92281-104">Hvis du har modtaget denne besked, er her de trin, der skal undersøges:</span><span class="sxs-lookup"><span data-stu-id="92281-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="92281-105">Fra beskeden skal du klikke på **Vis besked** for at gå til siden **beskeder** i sikkerheds & overholdelses Center.</span><span class="sxs-lookup"><span data-stu-id="92281-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="92281-106">Vælg beskeden for at se muligheden for at **få vist meddelelseslisten** eller **Se meddelelser i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="92281-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="92281-107">Begge disse indstillinger fører dig til detaljerne i meddelelsen, som omfatter meddelelses-id'et.</span><span class="sxs-lookup"><span data-stu-id="92281-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="92281-108">Bemærk, at linket til trussels Stifinder automatisk filtrerer de meddelelser, der opfylder beskedkriterierne.</span><span class="sxs-lookup"><span data-stu-id="92281-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="92281-109">Det kan være nødvendigt at justere datofiltret i trussels Stifinder.</span><span class="sxs-lookup"><span data-stu-id="92281-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="92281-110">Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:</span><span class="sxs-lookup"><span data-stu-id="92281-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="92281-111">En tilladt afsender eller et domæne, der er angivet af brugeren.</span><span class="sxs-lookup"><span data-stu-id="92281-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="92281-112">En tilladt afsender eller et domæne, der er angivet af administratoren i en antispam-politik.</span><span class="sxs-lookup"><span data-stu-id="92281-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="92281-113">En tilladt IP-adresse i en forbindelses filter politik.</span><span class="sxs-lookup"><span data-stu-id="92281-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="92281-114">En mail flow regel (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.</span><span class="sxs-lookup"><span data-stu-id="92281-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="92281-115">Hvis du mener, at meddelelsen er markeret forkert som Phish, skal du bruge [tilføjelsesprogram til Outlook-rapport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til at sende meddelelser til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92281-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
