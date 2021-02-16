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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256748"
---
# <a name="device-writeback"></a>Tilbageførsel af enhed

Tilbageførsel af enhed bruges i følgende scenarier:

- Aktivér [Windows Hello til virksomheder ved hjælp af installation af hybridcertifikattillid](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivér Betinget adgang baseret på enheder til ADFS (2012 R2 eller nyere) beskyttede programmer (afhængigt af parttillider)

    > [!NOTE]
    > Der kræves et abonnement på Azure AD Premium for tilbageskrivning af enheder.

Dette giver yderligere sikkerhed og sikkerhed for, at adgang til programmer kun gives til enheder, der er tillid til. Du kan finde flere [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) oplysninger om Betinget adgang under Administration af risici med Betinget adgang og Konfiguration af betinget adgang i det lokale miljø ved hjælp af [Registrering af Azure Active Directory-enheder.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Du kan finde flere oplysninger om aktivering af tilbageførsel af enheder for enheder under [Aktivér tilbageførsel af enhed.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
