---
title: Forberedelse til brug af TLS 1.2 i Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040392"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Forberedelse til brug af TLS 1.2 i Microsoft 365

Pr. 31. oktober 2018 fortsætter Microsoft 365 overgangen til TLS 1.2. Pr. 15. oktober 2020 begynder udrådningen af TLS 1.0 og 1.1 på tværs af tjenesten. Rullen af denne ændring vil fortsætte i løbet af de næste par uger og måneder, men kunder bør antage, at ingen TLS 1.0/1.1-opkald vil fungere, når de interagerer med O365 fra den 15. oktober 2020. Som det tidligere er meddelt (MC126199 i dec 2017, MC128929 i februar 2018, MC186827 i juli 2019 og MC218794 i juli 2020) flytter alle vores onlinetjenester til Transport Layer Security (TLS) 1.2+ for at levere førsteklasses kryptering og for at sikre, at vores tjeneste som standard er mere sikker. Kunder kan stadig vælge at have TLS 1.0/1.1 på deres servere og ressourcer, men de skal antage, at det kun er TLS 1.2 eller nyere, der fungerer, når de interagerer med O365-ressourcer.
  
Du kan få mere at vide om disse ændringer [her](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) og [her.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)

  