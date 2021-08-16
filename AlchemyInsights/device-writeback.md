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
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101944"
---
# <a name="device-writeback"></a>Tilbageførsel af enhed

Tilbageførsel af enhed bruges i følgende scenarier:

- Aktivere [Windows Hello for Business ved hjælp af hybridinstallation af certifikattillid](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivér Betinget adgang baseret på enheder med ADFS (2012 R2 eller nyere) beskyttede programmer (afhængig af parttillide)

    > [!NOTE]
    > Der kræves et Azure AD Premium for at tilbageførsel af enhed.

Dette giver yderligere sikkerhed for, at adgang til programmer kun gives til enheder, der er tillid til. Du kan finde flere [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) oplysninger om betinget adgang i Administrer risiko med betinget adgang og Konfiguration af betinget adgang i det lokale miljø ved [Azure Active Directory af Enhedsregistrering.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Du kan finde flere oplysninger om aktivering af tilbageførsel af enheder for enheder under [Aktivér tilbageførsel af enhed.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
