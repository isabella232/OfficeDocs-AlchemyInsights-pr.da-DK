---
title: Løse almindelige problemer med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930055"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Løse almindelige problemer med DKIM-postformatering

De fleste problemer med DKIM-konfigurationen er relateret til forkerte DNS-poster.

For at løse problemer med DKIM-opsætningen skal du kontrollere, at DKIM CNAME-posten **(** ikke en TXT-post) er formateret korrekt. Du kan finde flere [oplysninger under Hvad du skal gøre for at konfigurere DKIM manuelt i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Hvis du har brug for generel hjælp til DNS-poster, kan du [se Oprette DNS-poster for din DNS-udbyder Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Når du har oprettet eller opdateret dine DKIM DNS-poster hos DNS-hostingtjenesten for dit domæne, skal du vente på, at DNS-posterne overføres.
