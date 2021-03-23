---
title: Beskyttelse mod Backscatter-angreb
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035409"
---
# <a name="protection-from-backscatter-attack"></a>Beskyttelse mod Backscatter-angreb

Backscatter er rapporter om manglende levering (også kaldet rapporter om manglende levering eller meddelelser om ikke-leveret mail), som du modtager for meddelelser, du ikke har sendt. Afsendere af uønsket mail (spoof) **Fra:-adressen** på deres meddelelser, og de bruger ofte reelle mailadresser til at give deres meddelelser troværdighed. Så når spammere uundgåeligt sender meddelelser til ikke-eksisterende modtagere, bliver destinationsmailserveren i bund og grund narret til at returnere den meddelelse, der ikke kan leveres, i en NDR til den smedede afsender i **Fra:-adressen.**

Du kan finde flere oplysninger [i Backscatter i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**Aktivering af Backscatter-beskyttelse**

Følg stien nedenfor for at aktivere Backscatter-beskyttelse.

**protection.office.com > trusselsadministration > politik > antispam > Vælg politik for spamfilter og rediger politik > egenskaber > Spam > Markér som spam > NDR-backscatter > Indstil den til "Til"**

Hvis du mener, at en konto er blevet kompromitteret, skal du se følgende:

- [Besvare en kompromitteret mailkonto](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Fjerne blokerede brugere fra portalen Begrænsede brugere i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



