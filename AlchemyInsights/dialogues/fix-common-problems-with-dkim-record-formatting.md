---
title: Løs almindelige problemer med DKIM-postformatering
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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523748"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Løs almindelige problemer med DKIM-postformatering

De fleste problemer med DKIM-konfiguration er relateret til forkerte DNS-poster.

For at løse problemer med DKIM-opsætningen skal du kontrollere, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt. Du kan finde flere oplysninger [under Hvad du skal gøre for at konfigurere DKIM manuelt i Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Hvis du har brug for generel hjælp til DNS-poster, kan du se [Oprette DNS-poster for Office 365 hos](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)en hvilken som helst DNS-udbyder.

> [!NOTE]
> Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne, skal du vente på, at DNS-posterne bliver overført.
