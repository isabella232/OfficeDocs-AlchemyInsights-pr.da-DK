---
title: 305 Forøg størrelsen på arkivpostkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36661794"
---
# <a name="increase-the-archive-mailbox-size"></a>Forøge størrelsen på arkivpostkassen

Office 365 [begrænser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) størrelsen på arkivpostkasser baseret på den licens, der er tildelt brugerkontoen. Når arkivpostkassen når 90% af den tilladte størrelse, modtager brugeren en e-mail-meddelelse. Når en arkivpostkasse når sin størrelsesgrænse, kan brugeren ikke flytte flere elementer til arkivpostkassen. Office 365 øger ikke størrelsen på en arkivpostkasse, når størrelsesgrænsen er nået. I stedet kan brugerne foretage følgende handlinger for at frigøre plads i arkivpostkassen:

- Eksporter elementerne til en. pst-fil ved hjælp af Outlook.

- Slet elementer fra arkivpostkassen.

Office 365 giver **ubegrænset arkivering** til Office 365 Enterprise E3-og E5-licenser. En administrator skal aktivere denne funktion, før arkivpostkassen når sin maksimale størrelse. Når ubegrænset arkivering er aktiveret, kan det tage op til 30 dage, før der føjes ledig plads til arkivpostkassen. Derfor anbefaler vi, at administratorer kontrollerer den frie plads i arkivpostkassen, hvilket gør det muligt for brugeren at fortsætte med at bruge arkivpostkassen, mens den udvides. Du kan finde flere oplysninger under [Oversigt over ubegrænset arkivering i office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) og [aktivere ubegrænset arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Du finder flere oplysninger om, hvordan du får adgang til arkivpostkassen fra Outlook, under [Outlook-krav til adgang til elementer i et automatisk udvidet Arkiv](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Hvis du vil konfigurere en opbevaringspolitik, der automatisk flytter elementer til arkivpostkassen, skal du se [konfigurere en politik for arkivering og sletning af postkasser i din Office 365-organisation](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Bemærk**: automatisk udvidelse af arkiver understøttes ikke for primære postkasser på Exchange 2010.
