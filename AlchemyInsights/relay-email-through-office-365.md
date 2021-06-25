---
title: Videresend mails via Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117977"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="e4aad-102">Konfigurer en flerfunktionsenhed eller -program til at sende mail</span><span class="sxs-lookup"><span data-stu-id="e4aad-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="e4aad-103">Se dine muligheder og fremgangsmåden under [Sådan konfigurerer du flerfunktionsenheder eller -programmer til at sende mails ved hjælp af Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="e4aad-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="e4aad-104">Hvis du har en enhed eller et program, der for nyligt er holdt op med at fungere, er de mest almindelige problemer:</span><span class="sxs-lookup"><span data-stu-id="e4aad-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="e4aad-105">**Godkendelsesrelaterede fejl ved brug af SMTP-godkendt klientindsendelse** Vi har for nylig foretaget nogle ændringer i forbindelse med, hvordan SMTP-godkendelse fungerer.</span><span class="sxs-lookup"><span data-stu-id="e4aad-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="e4aad-106">Du kan finde flere oplysninger om, hvordan du løser problemer, i afsnittet Løs problemer med godkendelse uden held i afsnittet Løs problemer med [printere, scannere og LOB-programmer,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)der sender mails ved hjælp af Microsoft 365 eller Office 365.</span><span class="sxs-lookup"><span data-stu-id="e4aad-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="e4aad-107">**Vi accepterer kun TLS 1.2-versionen, mens vi laver en sikker forbindelse til Office 365** Hvis du bruger en sikker forbindelse (TLS), skal du kontrollere, at din programenhed understøtter TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="e4aad-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="e4aad-108">Du kan finde flere oplysninger [i Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="e4aad-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="e4aad-109">Hvis du vil have mere at vide om andre problemer og løsninger, skal du se Løs problemer med [printere, scannere](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)og LOB-programmer, der sender mails ved hjælp Microsoft 365 eller Office 365 .</span><span class="sxs-lookup"><span data-stu-id="e4aad-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="e4aad-110">For at se påvirkede enheder skal du gå til [rapporten for SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="e4aad-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="e4aad-111">**Bemærk:** Exchange Online ikke plads til scenarier med masseforsendelse.</span><span class="sxs-lookup"><span data-stu-id="e4aad-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="e4aad-112">Hvis du vil sende kommercielle massemails (f.eks. kundebrevbrev), skal du bruge tredjepartsudbydere, der er specialiserede i disse tjenester.</span><span class="sxs-lookup"><span data-stu-id="e4aad-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
