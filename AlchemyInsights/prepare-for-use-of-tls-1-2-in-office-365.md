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
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085898"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Forberedelse til brug af TLS 1.2 i Microsoft 365

Pr. 31. oktober 2018 fortsætter Microsoft 365 overgangen til TLS 1.2. Fra og med den 15. oktober 2020 starter O365 det frarådes at TLS 1,0 og 1,1 på tværs af tjenesten. Gennemførelsen af denne ændring vil fortsætte over de næste par uger og måneder, men kunder vil ikke kunne antage, at TLS 1.0/1.1-opkald fungerer, når de engagerer med O365, der starter okt 15, 2020. Som tidligere blevet kommunikeret (MC126199 i dec 2017, MC128929 i februar 2018, MC186827 i juli 2019 og MC218794 i juli 2020) gør vi alle vores onlinetjenester til transport Layer Security (TLS) 1.2 + for at sikre den bedst mulige kryptering og for at sikre, at vores tjeneste er mere sikker, som standard. Kunder kan stadig vælge at have TLS 1.0/1.1 på deres servere og ressourcer, men de bør kun antage, at TLS 1,2 eller nyere fungerer, når du interagerer med O365-ressourcer.
  
Hvis du vil have mere at vide om disse ændringer, skal du se [her](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) og [her](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  