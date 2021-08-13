---
title: Fejlfinding af brugersamtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007892"
---
# <a name="troubleshoot-user-consent"></a>Fejlfinding af brugersamtykke

1. Du kan konfigurere, hvordan slutbrugere giver deres samtykke til programmer via Azure-portalen eller PowerShell. Se Indstillinger [for brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for at få flere oplysninger.
1. En administrator kan også bruge [Microsofts Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til at give samtykke til delegerede tilladelser på vegne af en enkelt bruger. Du kan få mere at vide [under Få adgang på vegne af en bruger](https://docs.microsoft.com/graph/auth-v2-user).
1. [Fejl i brugersamtykke:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)I denne artikel beskrives fejl, der kan opstå under processen med at acceptere et program. Hvis du foretager fejlfinding af uventede samtykkeprompter, der ikke indeholder fejlmeddelelser, skal du [se Godkendelsesscenarier for Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)