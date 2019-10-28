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
ms.openlocfilehash: 08904708dd19104179c3f97f6734d8af725a4512
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745427"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a>Anbefalede trin, du skal udføre, hvis en konto er blevet kompromitteret

[VIDEO: Rettelse af en kompromitteret Office 365-konto](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. [Nulstil brugerens adgangskode](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) med det samme. Send ikke den nye adgangskode til slutbrugeren via mail.

2. Fjern alle mistænkelige [videresendelsesadresser](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding), der er angivet på postkasseniveauet.

3. Fjern alle mistænkelige [indbakkeregler](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED), der er angivet i postkassen.

4. Hvis brugeren er blevet blokeret og ikke kan sende mails, skal du [gå til siden Brugere med begrænset adgang for at fjerne blokeringen af kontoen](https://protection.office.com/?hash=/restrictedusers). Når du har gjort dette, bør brugeren kunne afsende mails fra kontoen igen inden for én time.

5. Fjern brugerkontoen fra alle [grupper for administrationsroller](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles), indtil du er sikker på, at kontoen ikke længere er kompromitteret.

For at minimere sandsynligheden for et databrud eller en kompromitteret konto i fremtiden, anbefaler vi, at du læser vores [Office 365-sikkerhedsplan ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).
  