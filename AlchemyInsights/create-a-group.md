---
title: Opret en gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088688"
---
# <a name="create-a-group"></a>Opret en gruppe

I dette emne beskrives gruppe oprettelse.

**Tilladelse til at oprette en gruppe**

Sørg for, at du har tilladelse til at oprette en ny gruppe. Globale administratorer kan deaktivere gruppe oprettelse i Azure-portalen eller Access-panelet. Du skal muligvis have en administrator for at oprette den nye gruppe for dig, eller for at give dig de relevante tilladelser.

**Administrer tilladelser til gruppe oprettelse**

1. Globale administratorer kan administrere tilladelser til gruppe oprettelse (for sikkerhedsrelaterede årsager) eller Office 365-grupper, der er oprettet i Azure-portalen eller Access-panelet, ved at vælge "brugerne kan oprette sikkerhedsgrupper i Azure-portaler" eller "brugerne kan oprette Office 365-grupper i Azure-portaler" i **alle grupperne**  >  **Generelt (indstillinger)**.
2. Du kan også begrænse oprettelse af gruppe for at vælge en gruppe af brugere, hvis du har en Azure Active Directory P1 Premium-licens.

**Deaktivering af velkomstmeddelelse for nye Office 365-gruppemedlemmer**

Den velkomstmeddelelse, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at angive **UnifiedGroupWelcomeMessageEnabled** til falsk i PowerShell. Få mere at vide om denne indstilling [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

