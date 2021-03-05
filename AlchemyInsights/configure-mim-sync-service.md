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
# <a name="configure-mim-sync-service"></a><span data-ttu-id="046e8-102">Konfigurere MIM-synkroniseringstjeneste</span><span class="sxs-lookup"><span data-stu-id="046e8-102">Configure MIM Sync service</span></span>

<span data-ttu-id="046e8-103">Synkroniseringstjenesten til Microsoft Identity Manager (MIM) er en komponent i MIM.</span><span class="sxs-lookup"><span data-stu-id="046e8-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="046e8-104">Det er en centraliseret lokal tjeneste, der lagrer og integrerer oplysninger for organisationer, der har flere lokale mapper og databaser.</span><span class="sxs-lookup"><span data-stu-id="046e8-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="046e8-105">Du kan muligvis løse dit problem med MIM-synkronisering, hvis problemet blev løst i en nylig opdatering til MIM, eller er et af de andre problemer, der er nævnt i nedenstående afsnit.</span><span class="sxs-lookup"><span data-stu-id="046e8-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="046e8-106">**Anbefalede trin**</span><span class="sxs-lookup"><span data-stu-id="046e8-106">**Recommended steps**</span></span>

1. <span data-ttu-id="046e8-107">Sørg for, at du bruger en nylig opdatering af MIM-synkronisering, og kontrollér produktbemærkningerne til [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) for at finde ud af, om problemet er løst i en opdatering.</span><span class="sxs-lookup"><span data-stu-id="046e8-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="046e8-108">Hvis problemet er med forbindelseskomponent Generic LDAP, Generic SQL, Lotus Domino eller Web Services, skal du sikre dig, at du bruger en nylig opdatering af [de generiske forbindelser.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="046e8-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="046e8-109">Hvis en MIM-synkroniseringskørsel stopper med en fejl, skal du se tabellen over [kørselsfejlkoder for](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) at finde de mulige årsager.</span><span class="sxs-lookup"><span data-stu-id="046e8-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="046e8-110">Hvis kørslen stopper med **filtypenavnet dll-undtagelse,** skal  du klikke på disse ord for at åbne vinduet Egenskaber for forbindelsespladsobjekt og klikke på **Staksporing...** for at få vist flere oplysninger om den underliggende årsag som beskrevet i [Filtypenavn-DLL-undtagelse.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)</span><span class="sxs-lookup"><span data-stu-id="046e8-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="046e8-111">Hvis pcNS-komponenten (Password Change Notification Service) rapporterer fejl **6025** i hændelsesloggen under synkronisering af adgangskoder, skal du se vejledningen til fejlfinding af [PCNS-rapporteringsfejl 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="046e8-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="046e8-112">Hvis fuld synkronisering med FIM-servicestyringsagenten er langsom, skal du kontrollere indstillingen for automatisk vækst for TempDB som beskrevet i Fejlfinding i langsom [eller hængende fuld synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) </span><span class="sxs-lookup"><span data-stu-id="046e8-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="046e8-113">Hvis du støder på en fejl i en afbrudt server med mislykket oprettelse-via-web-tjenester ved hjælp af FIM Service Management Agent, skal du se [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for en oversigt over årsager.</span><span class="sxs-lookup"><span data-stu-id="046e8-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

