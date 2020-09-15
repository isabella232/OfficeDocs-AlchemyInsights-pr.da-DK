---
title: 'Fejl: reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690957"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fejl: reglerne på denne computer stemmer ikke overens

Hvis du vil se en opdateret status for dette kendte problem, skal du se [reglerne på denne computer stemmer ikke overens med reglerne på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementeret en rettelse i Build 12928,10000. Rettelsen er allerede i insider fast og vil gå til månedlig kanal i den sene juni 2020. Når du har den faste build, kan du få meddelelsen "hvilke regler vil du gemme" en sidste gang. Vælg server, når du bliver bedt om det, og gå derefter tilbage til Outlook, og Aktivér eventuelle regler, der er deaktiveret.

Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:

**Løsning**: der er opstået et problem i de seneste rapporter for de personer, der kun har oprettet klientregler i Outlook på computeren. Hvis du fortsat kører i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.

Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook ved at køre Outlook.exe/Cleanrules. Dette vil slette både klient-og server reglerne. Den vil slette alle reglerne for alle konti i Outlook-profilen. Denne kommando er yderligere dokumenteret i artiklen kommandolinjeparametre.

