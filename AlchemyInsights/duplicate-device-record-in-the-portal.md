---
title: Dupliker enhedspost i-portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678498"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dupliker enhedspost i-portalen

Du kan få vist 2 poster for en enhed i-portalen, hvis enheden ikke korrekt rapporterer status for fælles administration på Konfigurationsstyringswebstedet. Hvis du vil kontrollere en enheds administrationsstatus, skal du gennemse kolonnen **Fælles administreret** for enheden i Konfigurationsstyringskonsollen. Hvis kolonnen ikke er synlig, kan du tilføje den ved at højreklikke på en af kolonneoverskrifterne og markere den på listen.

Den fællesadministrerede værdi skal være **Ja**.. Hvis værdien er **Nej**, skal du åbne Konfigurationsstyring-klient-applet på klientenheden og markere egenskaben **Fælles administration** på Generel-fanen.

- Hvis værdien er **Aktiveret**, indikerer dette, at der er problemer med klientkommunikationen med Administrationspunktet. Gennemse **CcmMessaging.log** på enheden for at undersøge potentielle forbindelsesproblemer.

- Hvis værdien er Deaktiveret og enheden er tilmeldt i Intune, skal du sørge for, at enheden har modtaget politikken for fælles administration, ved at gennemgå **CoManagementHandler.log** på enheden.
