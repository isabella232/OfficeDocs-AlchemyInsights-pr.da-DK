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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427086"
---
# <a name="gpo-deployment"></a>Installation af gruppepolitikobjekt

Indstillinger for bruger- og computerobjekter i Azure Active Directory-domæneservices (Azure AD DS) administreres ofte ved hjælp af Gruppepolitik objekter (GPOs). Azure AD DS indeholder indbyggede GPOs til AADDC-brugere og AADDC-computerbeholdere. Du kan tilpasse disse indbyggede gruppepolitikobjekter for at konfigurere gruppepolitikken efter behov for dit miljø. Medlemmer af gruppen Azure AD DC-administratorer har gruppepolitikadministrationsrettigheder i Azure AD DS-domænet, og de kan også oprette brugerdefinerede GRUPPE'er og organisationsenheder. Du kan finde flere oplysninger om, hvad gruppepolitik er, og hvordan den [fungerer, Gruppepolitik Oversigt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I et hybridmiljø synkroniseres gruppepolitikker, der er konfigureret i et lokalt AD DS miljø, ikke med Azure AD DS. Hvis du vil definere konfigurationsindstillinger for brugere eller computere i Azure AD DS, skal du redigere et af standard-GRUPPEpolitikobjekter eller oprette et brugerdefineret gruppepolitikobjekt.

I denne artikel [administreres Gruppepolitik,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hvordan du installerer Gruppepolitik-administrationsværktøjerne, hvordan du redigerer de indbyggede gruppepolitikobjekter, og hvordan du opretter brugerdefinerede gruppepolitikobjekter.
