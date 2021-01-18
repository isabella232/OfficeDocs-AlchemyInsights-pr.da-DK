---
title: Virtuel konfiguration med AAD-domæne tjenester
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884975"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuel konfiguration med AAD-domæne tjenester

Virtuel konfiguration med AAD-domæne tjenester involverer følgende trin: 

1. Kontrollere domænets tilstand på Azure-portalen https://aka.ms/aadds-health
2. Kontrollér din NSG for regler, der blokerer de porte, der kræves for at synkronisere i Azure AD-domæne tjenester på portalen https://aka.ms/aadds-networking
3. Sikre, at dit virtuelle netværk er installeret i det samme Azure-område som dit Azure AD Domain Services-administreret domæne.
4. Sørg for, at du ikke har et eksisterende domæne med det samme domænenavn, der er tilgængeligt på det virtuelle netværk.

Du kan finde flere oplysninger om Designovervejelser i Azure virtuelt netværk, der understøtter AAD-domæne tjenester, under overvejelser i forbindelse med [virtuelt netværk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

