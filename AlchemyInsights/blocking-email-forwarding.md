---
title: Bloker eller fjern blokeringen af ekstern automatisk videresendelse af mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897462"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloker eller fjern blokeringen af automatisk videresendelse af mail

Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du [se Konfigurer videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Administratorer kan styre ekstern videresendelse for organisationen ved hjælp af politikker for [udgående spam.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Du administrerer politikker for udgående spam i Microsoft 365 Defender-portalen på eller ved hjælp af <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy-cmdlet'en](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online PowerShell.

Hvis du får vist følgende fejlmeddelelse: **"550 5.7.520 Access denied, Your organization does not allow external forwarding",** make sure the policy is configured to enable external auto-forwarded messages.

**Bemærk!** Vi anbefalede standardværdien Automatisk –  **Systemet** styres for indstillingen for automatisk videresendelse i din standardpolitik for udgående spamfilter (automatisk ekstern videresendelse er blokeret. Intern automatisk videresendelse fungerer stadig). Du bør oprette brugerdefinerede politikker for udgående spamfilter og bruge værdien Til **–** Videresendelse er kun aktiveret for brugere, der har brug for ekstern automatisk videresendelse af mail. Du kan få mere at vide [under Konfiguration af ekstern videresendelse af mail Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
