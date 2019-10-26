---
title: Videresend mails via Office 365
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
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745391"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="383ef-102">Konfigurer en flerfunktionsenhed eller -program til at sende mails ved hjælp af Office 365</span><span class="sxs-lookup"><span data-stu-id="383ef-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="383ef-103">Se dine muligheder og fremgangsmåden under [Sådan konfigurerer du flerfunktionsenheder eller -programmer til at sende mails ved hjælp af Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="383ef-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="383ef-104">**Bemærk:** Hvis du har en enhed eller et program, der for nylig er holdt op med at virke, bør du bemærke, at vi for nyligt er begyndt at [deaktivere 3DES kryptering](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) som planlagt.</span><span class="sxs-lookup"><span data-stu-id="383ef-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="383ef-105">For at se påvirkede enheder skal du gå til [rapporten for SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="383ef-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="383ef-106">Almindelige fejl kan være i stil med: godkendelsesfejl, TLS-fejl, fejl i krypteringsalgoritme, uoverensstemmelse med algoritme eller tabt forbindelse.</span><span class="sxs-lookup"><span data-stu-id="383ef-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="383ef-107">Sådan løser du problemet:</span><span class="sxs-lookup"><span data-stu-id="383ef-107">To resolve the issue:</span></span>
 - <span data-ttu-id="383ef-108">**Windows Server 2003 IIS SMTP fungerer ikke længere – der kræves en nyere version af Windows.**</span><span class="sxs-lookup"><span data-stu-id="383ef-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="383ef-109">Kontakt venligst din leverandør af programmet eller enheden for at finde ud af, om en moderne kryptering understøttes, eller om der er en opdatering.</span><span class="sxs-lookup"><span data-stu-id="383ef-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
