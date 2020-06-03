---
title: Anbefalede trin, du skal udføre, hvis en konto er blevet kompromitteret
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: a094862a175184c3ac2a717cc59aefe2470b9fd1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510782"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a>Anbefalede trin, du skal udføre, hvis en konto er blevet kompromitteret

[VIDEO: Rettelse af en kompromitteret konto](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. [Nulstil brugerens adgangskode](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) med det samme. Send ikke den nye adgangskode til slutbrugeren via mail.

2. Fjern alle mistænkelige [videresendelsesadresser](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding), der er angivet på postkasseniveauet.

3. Fjern alle mistænkelige [indbakkeregler](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED), der er angivet i postkassen.

4. Hvis brugeren er blevet blokeret og ikke kan sende mails, skal du [gå til siden Brugere med begrænset adgang for at fjerne blokeringen af kontoen](https://protection.office.com/?hash=/restrictedusers). Når du har gjort dette, bør brugeren kunne afsende mails fra kontoen igen inden for én time.

5. Fjern brugerkontoen fra alle [grupper for administrationsroller](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles), indtil du er sikker på, at kontoen ikke længere er kompromitteret.

For at minimere sandsynligheden for et databrud eller en kompromitteret konto i fremtiden, anbefaler vi, at du læser vores [Microsoft 365-sikkerhedsplan ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).
  