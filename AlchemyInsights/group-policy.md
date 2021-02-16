---
title: Gruppepolitik
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256682"
---
# <a name="group-policy"></a>Gruppepolitik

Indstillinger for bruger- og computerobjekter i Azure Active Directory-domæneservices (Azure AD DS) administreres ofte ved hjælp af Gruppepolitik objekter (GPOs). Azure AD DS indeholder indbyggede GPOs til AADDC-brugere og AADDC-computerbeholdere. Du kan tilpasse disse indbyggede gruppepolitikobjekter for at konfigurere gruppepolitikken efter behov for dit miljø. Medlemmer af gruppen Azure AD DC-administratorer har gruppepolitikadministrationsrettigheder i Azure AD DS-domænet, og de kan også oprette brugerdefinerede GRUPPE'er og organisationsenheder. Du kan finde flere oplysninger om, hvad gruppepolitik er, og hvordan den [fungerer, Gruppepolitik oversigt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I et hybridmiljø synkroniseres gruppepolitikker, der er konfigureret i et lokalt AD DS miljø, ikke med Azure AD DS. Hvis du vil definere konfigurationsindstillinger for brugere eller computere i Azure AD DS, skal du redigere et af standard-GRUPPEpolitikobjekter eller oprette et brugerdefineret gruppepolitikobjekt.

I denne artikel [administreres Gruppepolitik,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hvordan du installerer Gruppepolitik-administrationsværktøjerne, hvordan du redigerer de indbyggede gruppepolitikobjekter, og hvordan du opretter brugerdefinerede gruppepolitikobjekter.



