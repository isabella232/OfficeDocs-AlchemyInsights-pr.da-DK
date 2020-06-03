---
title: Videresend mails via Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 727fa38233697c778caa9325b2671501cb75d5fd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510710"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="38cc0-102">Konfigurer en flerfunktionsenhed eller -program til at sende mail</span><span class="sxs-lookup"><span data-stu-id="38cc0-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="38cc0-103">Se dine muligheder og fremgangsmåden under [Sådan konfigurerer du flerfunktionsenheder eller -programmer til at sende mails ved hjælp af Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="38cc0-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="38cc0-104">**Bemærk:** Hvis du har en enhed eller et program, der for nylig er holdt op med at virke, bør du bemærke, at vi for nyligt er begyndt at [deaktivere 3DES kryptering](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) som planlagt.</span><span class="sxs-lookup"><span data-stu-id="38cc0-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="38cc0-105">For at se påvirkede enheder skal du gå til [rapporten for SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="38cc0-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="38cc0-106">Almindelige fejl kan være i stil med: godkendelsesfejl, TLS-fejl, fejl i krypteringsalgoritme, uoverensstemmelse med algoritme eller tabt forbindelse.</span><span class="sxs-lookup"><span data-stu-id="38cc0-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="38cc0-107">Sådan løser du problemet:</span><span class="sxs-lookup"><span data-stu-id="38cc0-107">To resolve the issue:</span></span>
 - <span data-ttu-id="38cc0-108">**Windows Server 2003 IIS SMTP fungerer ikke længere – der kræves en nyere version af Windows.**</span><span class="sxs-lookup"><span data-stu-id="38cc0-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="38cc0-109">Kontakt venligst din leverandør af programmet eller enheden for at finde ud af, om en moderne kryptering understøttes, eller om der er en opdatering.</span><span class="sxs-lookup"><span data-stu-id="38cc0-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
