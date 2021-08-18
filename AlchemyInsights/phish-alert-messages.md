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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316352"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Giv besked om mails fra politikken "Phish leveret på grund af lejer eller brugertilsidesættelse"

En standardbeskedpolitik, der hedder **Phish Leveret** pga. lejer eller brugertilsidesættelse, er tilgængelig i organisationer med Microsoft Defender til Office 365 P1- og P2-licenser. Hvis du har modtaget denne besked, skal du undersøge følgende:

1. I beskeden skal du klikke på **Vis besked** for at gå **til siden** Vigtige beskeder Microsoft 365 Defender portalen.

2. Vælg beskeden for at få vist indstillingen Vis **meddelelsesliste eller** **Vis meddelelser i Stifinder.** Begge disse indstillinger giver dig adgang til detaljerne i meddelelsen, som indeholder meddelelses-id'et. Bemærk, at linket Threat Explorer automatisk filtrerer de meddelelser, der opfylder beskedkriterierne. Du skal muligvis justere datofilteret i Threat Explorer.

Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:

- En tilladt afsender eller et domæne, der er angivet af brugeren.
- En tilladt afsender eller et domæne, der er angivet af administratoren i en politik for uønsket post.
- En tilladt IP-adresse i en forbindelsesfilterpolitik.
- En regel for mailflow (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.

Hvis du mener, at meddelelsen er forkert markeret som phishing, kan du bruge [administratorindsendelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) til at rapportere meddelelsen til Microsoft.

Brugerne kan bruge tilføjelsesprogrammet Rapportmeddelelse eller tilføjelsesprogrammet [Rapportphishing i](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Outlook sende meddelelseseksempler til Microsoft.
