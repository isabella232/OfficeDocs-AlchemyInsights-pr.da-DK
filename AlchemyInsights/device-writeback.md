---
title: Tilbageførsel af enhed
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320080"
---
# <a name="device-writeback"></a>Tilbageførsel af enhed

Tilbageførsel af enhed bruges i følgende scenarier:

- Aktivere [Windows Hello for Business ved hjælp af hybridinstallation af certifikattillid](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivér Betinget adgang baseret på enheder med ADFS (2012 R2 eller nyere) beskyttede programmer (afhængig af parttillide)

    **Bemærk!** Der kræves et Azure AD Premium for at tilbageførsel af enhed.

Dette giver yderligere sikkerhed for, at adgang til programmer kun gives til enheder, der er tillid til. Du kan finde flere [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) oplysninger om Betinget adgang i Administrer risiko med betinget adgang og Konfiguration af betinget adgang i det lokale miljø [ved Azure Active Directory af enhedsregistrering.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Du kan finde flere oplysninger om aktivering af tilbageførsel af enheder for enheder under [Aktivér tilbageførsel af enhed.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
