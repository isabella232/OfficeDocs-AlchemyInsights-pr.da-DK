---
title: Problem med sikkerhedsgrupper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177419"
---
# <a name="issue-with-security-groups"></a>Problem med sikkerhedsgrupper

**Hvis du får netværksfejlen AADDS104**

Ugyldige regler for netværkssikkerhedsgruppe er den mest almindelige årsag til netværksfejl i Azure Active Directory-domæneservices (AD DS). Netværkssikkerhedsgruppen for det virtuelle netværk skal tillade adgang til bestemte porte og protokoller. Hvis disse porte blokeres, kan Azure-platformen ikke overvåge eller opdatere det administrerede domæne. Synkroniseringen mellem Azure AD og Azure AD DS påvirkes også. Sørg for, at standardportene er åbne for at undgå afbrydelser af tjenesten.

Hvis du vil forstå og løse almindelige beskeder om konfigurationsproblemer med netværkssikkerhedsgrupper, skal du [se Tilføj og Bekræft sikkerhedsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
