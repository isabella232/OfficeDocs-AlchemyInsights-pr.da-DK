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
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Giv mails besked fra politikken "leveret, der er leveret på grund af leje-eller bruger tilsidesættelse"

En standard besked politik med navnet "Phish leveret på grund af leje-eller bruger tilsidesættelse" er blevet udrullet til lejere med Office 365 DTT-licenser og P2-licenser. Hvis du har modtaget denne besked, er her de trin, der skal undersøges:

1. Fra beskeden skal du klikke på **Vis besked** for at gå til siden **beskeder** i sikkerheds & overholdelses Center.

2. Vælg beskeden for at se muligheden for at **få vist meddelelseslisten** eller **Se meddelelser i Stifinder**. Begge disse indstillinger fører dig til detaljerne i meddelelsen, som omfatter meddelelses-id'et. Bemærk, at linket til trussels Stifinder automatisk filtrerer de meddelelser, der opfylder beskedkriterierne. Det kan være nødvendigt at justere datofiltret i trussels Stifinder.

Phishing-meddelelsen blev leveret på grund af en manuelt konfigureret tilsidesættelse:

- En tilladt afsender eller et domæne, der er angivet af brugeren.

- En tilladt afsender eller et domæne, der er angivet af administratoren i en antispam-politik.

- En tilladt IP-adresse i en forbindelses filter politik.

- En mail flow regel (også kaldet en transportregel), der er konfigureret til at tillade meddelelser i.

Hvis du mener, at meddelelsen er markeret forkert som Phish, skal du bruge [tilføjelsesprogram til Outlook-rapport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til at sende meddelelser til Microsoft.
