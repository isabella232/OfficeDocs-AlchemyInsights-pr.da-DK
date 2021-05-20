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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544572"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Giv besked om mails fra politikken "Phish leveret på grund af lejer eller brugertilsidesættelse"

En standardbeskedpolitik med navnet "Phish Leveret pga. lejer eller brugertilsidesættelse" er blevet udrullet til lejere med Microsoft Defender Office 365 P1- og P2-licenser. Hvis du har modtaget denne besked, skal du undersøge følgende:

1. I beskeden skal du klikke på **Vis besked** for at gå til **siden** Vigtige beskeder i & Security Compliance Center.

2. Vælg beskeden for at få vist indstillingen Vis **meddelelsesliste eller** **Vis meddelelser i Stifinder.** Begge disse indstillinger giver dig adgang til detaljerne i meddelelsen, som indeholder meddelelses-id'et. Bemærk, at linket Threat Explorer automatisk filtrerer de meddelelser, der opfylder beskedkriterierne. Du skal muligvis justere datofilteret i Threat Explorer.

Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:

- En tilladt afsender eller et domæne, der er angivet af brugeren.

- En tilladt afsender eller et domæne, der er angivet af administratoren i en politik for uønsket post.

- En tilladt IP-adresse i en forbindelsesfilterpolitik.

- En regel for mailflow (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.

Hvis du mener, at meddelelsen er forkert markeret som [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) phish, skal du bruge tilføjelsesprogrammet Rapportmeddelelse Outlook at sende meddelelseseksempler til Microsoft.
