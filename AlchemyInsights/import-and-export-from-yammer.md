---
title: Importér og eksportér fra Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035440"
---
# <a name="import-and-export-from-yammer"></a>Importér og eksportér fra Yammer

**Importér**

Indstillingerne for brugerimport varierer, afhængigt af Yammer dit netværk er i oprindelig [tilstand til Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller ej.

- **Ikke-indbygget tilstand:** Brugere kan importeres til grupper ved hjælp af Tilføj fra adressekartotek [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) [(grænse](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) til 100 brugere) i gruppeindstillinger eller til netværket ved hjælp af masseopdatering i netværksadministrator.
- **Indbygget** tilstand: Gruppemedlemskab og netværksmedlemskabshandlinger skal udføres fra [Microsoft 365-administrationsportalen,](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ved hjælp af en anden Azure AD-indstilling. Netværk i indbygget tilstand har ikke længere adgang til Masseopdatering og andre ældre funktioner.

> [!IMPORTANT]
> Yammer aldrig har understøttet import af indhold fra netværksadministrator, selv når funktionen Dataeksport blev brugt i et andet netværk. Indhold kan genopslås af partnerløsninger eller Yammer REST-API'er.

**Eksportér**

[Eksportér netværksdata i netværksadministrator](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillader eksport af indhold fra Yammer netværk, herunder meddelelser og filer. Vedhæftede filer kan være meget store og medføre, at eksporter tager lang tid at gennemføre. Vi anbefaler, at aktive netværk eksporteres ved hjælp af [dataeksport-API'en](https://developer.yammer.com/docs/data-export-api) i dele efter dag eller uge. Microsoft Support leverer ikke brugerdefinerede scripts til dette formål.

Der findes [en separat GDPR-eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) for at eksportere indhold til en enkelt bruger.