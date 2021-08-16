---
title: Installation af gruppepolitikobjekt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067834"
---
# <a name="gpo-deployment"></a>Installation af gruppepolitikobjekt

Indstillinger for bruger- og computerobjekter i Azure Active Directory-domænetjenester (Azure AD DS) administreres ofte ved hjælp af Gruppepolitik-objekter (GPOs). Azure AD DS indeholder indbyggede GPOs til AADDC-brugere og AADDC-computerbeholdere. Du kan tilpasse disse indbyggede GPOs til at konfigurere gruppepolitik efter behov for dit miljø. Medlemmer af administratorgruppen Azure AD DC-administratorer har gruppepolitikadministrationsrettigheder i Azure AD DS-domænet og kan også oprette brugerdefinerede GPOs og organisationsenheder (OUs). Du kan finde flere oplysninger om, hvad gruppepolitik er, og hvordan den fungerer, [Gruppepolitik Oversigt](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

I et hybridmiljø synkroniseres gruppepolitikker, der er konfigureret i AD DS lokalt miljø, ikke med Azure AD DS. For at definere konfigurationsindstillinger for brugere eller computere i Azure AD DS skal du redigere en af standard-GPOs eller oprette et brugerdefineret gruppepolitikobjekt.

I denne artikel kan [Gruppepolitik](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) se, hvordan du installerer Gruppepolitik-administrationsværktøjerne, hvordan du redigerer de indbyggede GPOs, og hvordan du opretter brugerdefinerede gpos.
