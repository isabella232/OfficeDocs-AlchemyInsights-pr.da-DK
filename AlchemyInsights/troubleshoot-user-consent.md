---
title: Foretag fejlfinding af brugersamtykke
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900961"
---
# <a name="troubleshoot-user-consent"></a>Foretag fejlfinding af brugersamtykke

1. Du kan konfigurere, hvordan slutbrugere skal have tilladelse til at bruge programmer via Azure-portalen eller PowerShell. Se [Indstillinger for brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for at få flere oplysninger.
1. En administrator kan også bruge [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til at give samtykke til uddelegerede tilladelser på vegne af en enkelt bruger. Hvis du vil have mere at vide, skal du se [få adgang på vegne af en bruger](https://docs.microsoft.com/graph/auth-v2-user).
1. [Fejl i brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): denne artikel omhandler fejl, der kan opstå under processen med at sende til et program. Hvis du foretager fejlfinding af uventede samtykke anmodninger, der ikke indeholder nogen fejlmeddelelser, skal du se [godkendelses scenarier for Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).