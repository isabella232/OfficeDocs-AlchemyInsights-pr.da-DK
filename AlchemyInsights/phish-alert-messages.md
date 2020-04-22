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
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Giv e-mails besked fra politikken "Phish Delivered due to tenant or user override"

En standardadvarselspolitik med navnet "Phish Delivered due to tenant or user override" er blevet udrullet til lejere med Office 365 ATP P1- og P2-licenser. Hvis du har modtaget denne besked, er her trinnene til at undersøge:

1. Klik på Vis **besked** i beskedbeskeden for at gå til siden **Beskeder** i Sikkerheds& Compliance Center.

2. Vælg beskeden for at få vist indstillingen **Vis meddelelsesliste** eller **Vis meddelelser i Stifinder**. Begge disse indstillinger tager dig til detaljerne i meddelelsen, som omfatter meddelelses-id'et. Bemærk, at linket Trusselsfinder automatisk filtrerer de meddelelser, der opfylder advarselskriterierne. Du skal muligvis justere datofilteret i Trusselstifinder.

Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:

- En tilladt afsender eller et tilladt domæne, der er angivet af brugeren.

- En tilladt afsender eller et tilladt domæne, der er indstillet af administratoren i en antispampolitik.

- En tilladt IP-adresse i en politik for forbindelsesfilter.

- En mailflowregel (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.

Hvis du mener, at meddelelsen er markeret forkert som phish, skal du bruge [tilføjelsesprogrammet Outlook-rapportmeddelelse](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til at sende meddelelseseksempler til Microsoft.
