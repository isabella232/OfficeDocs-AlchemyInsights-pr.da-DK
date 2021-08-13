---
title: 305 Øg arkivpostkassens størrelse
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926377"
---
# <a name="increase-the-archive-mailbox-size"></a>Øg arkivpostkassens størrelse


Hvis du vil have os til at køre automatiserede kontroller af de indstillinger, der er nævnt nedenfor, skal du vælge knappen Tilbage < – øverst på denne side og derefter angive mailadressen på den bruger, der skal have størrelsen på arkivpostkassen øget.

Microsoft 365 [begrænser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) størrelsen på arkivpostkasser baseret på den licens, der er tildelt brugerkontoen. Når arkivpostkassen når 90 % af dens tilladte størrelse, modtager brugeren en besked via mail. Når en arkivpostkasse når størrelsesgrænsen, kan brugeren ikke flytte flere elementer til arkivpostkassen. Microsoft 365 vil ikke øge størrelsen på en arkivpostkasse, når størrelsesgrænsen er nået. I stedet kan brugerne udføre følgende handlinger for at frigøre plads i arkivpostkassen:

- Eksportér elementerne til en .pst-fil ved hjælp Outlook.

- Slet elementer fra arkivpostkassen.

Microsoft 365 giver **ubegrænset arkivering** for Office 365 Enterprise E3- og E5-licenser. En administrator skal aktivere denne funktion, før arkivpostkassen når dens maksimale størrelse. Når ubegrænset arkivering er aktiveret, kan det tage op til 30 dage, før der føjes ledig plads til arkivpostkassen. Derfor anbefaler vi, at administratorer bekræfter den ledige plads i arkivpostkassen, så brugeren kan fortsætte med at bruge arkivpostkassen, mens den udvides. Få mere at vide under [Oversigt over ubegrænset arkivering i Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) [Aktivér ubegrænset arkivering i Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Du kan finde flere oplysninger om adgang til arkivpostkassen fra Outlook i Outlook for adgang til elementer i [et automatisk udvidet arkiv](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Hvis du vil konfigurere en opbevaringspolitik, der automatisk flytter elementer til arkivpostkassen, skal du se Konfigurer en arkiv- og sletningspolitik [for postkasser i din Microsoft 365 organisation.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**Bemærk!** Automatisk udvidende arkiver understøttes ikke for primære postkasser på Exchange 2010.
