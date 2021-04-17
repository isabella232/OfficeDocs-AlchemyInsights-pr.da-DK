---
title: Opret en gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816342"
---
# <a name="create-a-group"></a>Opret en gruppe

I dette emne beskrives oprettelse af grupper.

**Tilladelse til at oprette en gruppe**

Sørg for, at du er godkendt til at oprette en ny gruppe. Globale administratorer kan deaktivere oprettelse af grupper i Azure-portalen eller adgangspanelet. Du skal muligvis have en administrator for at oprette den nye gruppe for dig eller for at give dig de relevante tilladelser.

**Administrere tilladelser til oprettelse af grupper**

1. Globale administratorer kan administrere tilladelser til oprettelse af grupper (af sikkerhedsrelaterede årsager) eller Office 365-grupper, der er oprettet i Azure-portalen eller adgangspanelet, ved at vælge indstillingerne "Brugere kan oprette sikkerhedsgrupper i Azure-portaler" eller "Brugere kan oprette Office 365-grupper i Azure-portaler" i Alle grupper Generelt  >  **(Indstillinger).**
2. Du kan også begrænse oprettelse af grupper for at vælge en gruppe af brugere, hvis du har en Azure Active Directory P1 Premium-licens.

**Deaktivere velkomstmeddelelse for nye Office 365-gruppemedlemmer**

Velkomstmeddelelsen, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at angive **UnifiedGroupWelcomeMessageEnabled** til False i Powershell. Få mere at vide om denne [indstilling her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

