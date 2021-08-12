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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929299"
---
# <a name="create-a-group"></a>Opret en gruppe

I dette emne beskrives oprettelse af grupper.

**Tilladelse til at oprette en gruppe**

Sørg for, at du er godkendt til at oprette en ny gruppe. Globale administratorer kan deaktivere oprettelse af grupper i Azure-portalen eller adgangspanelet. Du skal muligvis have en administrator for at oprette den nye gruppe for dig eller for at give dig de relevante tilladelser.

**Administrere tilladelser til oprettelse af grupper**

1. Globale administratorer kan administrere tilladelser til oprettelse af grupper (af sikkerhedsrelaterede årsager) eller Office 365-grupper, der er oprettet i Azure-portalen eller adgangspanelet, ved at vælge indstillingerne "Brugere kan oprette sikkerhedsgrupper i Azure-portaler" eller "Brugere kan oprette Office 365-grupper i Azure-portaler" i Alle grupper Generelt  >  **(Indstillinger).**
2. Du kan også begrænse oprettelse af grupper for at vælge en gruppe af brugere, hvis du har en Azure Active Directory P1 Premium licens.

**Deaktiverer velkomstmeddelelse for nye Office 365 gruppemedlemmer**

Velkomstmeddelelsen, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at angive **UnifiedGroupWelcomeMessageEnabled** til Falsk i Powershell. Få mere at vide om denne [indstilling her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

