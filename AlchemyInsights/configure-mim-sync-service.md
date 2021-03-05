---
title: Konfigurere MIM-synkroniseringstjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481093"
---
# <a name="configure-mim-sync-service"></a>Konfigurere MIM-synkroniseringstjeneste

Synkroniseringstjenesten til Microsoft Identity Manager (MIM) er en komponent i MIM. Det er en centraliseret lokal tjeneste, der lagrer og integrerer oplysninger for organisationer, der har flere lokale mapper og databaser. Du kan muligvis løse dit problem med MIM-synkronisering, hvis problemet blev løst i en nylig opdatering til MIM, eller er et af de andre problemer, der er nævnt i nedenstående afsnit.

**Anbefalede trin**

1. Sørg for, at du bruger en nylig opdatering af MIM-synkronisering, og kontrollér produktbemærkningerne til [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) for at finde ud af, om problemet er løst i en opdatering.
2. Hvis problemet er med forbindelseskomponent Generic LDAP, Generic SQL, Lotus Domino eller Web Services, skal du sikre dig, at du bruger en nylig opdatering af [de generiske forbindelser.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Hvis en MIM-synkroniseringskørsel stopper med en fejl, skal du se tabellen over [kørselsfejlkoder for](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) at finde de mulige årsager.
4. Hvis kørslen stopper med **filtypenavnet dll-undtagelse,** skal  du klikke på disse ord for at åbne vinduet Egenskaber for forbindelsespladsobjekt og klikke på **Staksporing...** for at få vist flere oplysninger om den underliggende årsag som beskrevet i [Filtypenavn-DLL-undtagelse.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. Hvis pcNS-komponenten (Password Change Notification Service) rapporterer fejl **6025** i hændelsesloggen under synkronisering af adgangskoder, skal du se vejledningen til fejlfinding af [PCNS-rapporteringsfejl 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Hvis fuld synkronisering med FIM-servicestyringsagenten er langsom, skal du kontrollere indstillingen for automatisk vækst for TempDB som beskrevet i Fejlfinding i langsom [eller hængende fuld synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) 
7. Hvis du støder på en fejl i en afbrudt server med mislykket oprettelse-via-web-tjenester ved hjælp af FIM Service Management Agent, skal du se [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for en oversigt over årsager.

