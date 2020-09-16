---
title: Slette en privat kanal i teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730909"
---
# <a name="delete-a-teams-private-channel"></a>Slette en privat kanal i teams

Microsoft er opmærksom på et problem, der sletter en privat kanal for teams, hvis du har aktiveret SharePoint-opbevaringspolitikker for det underliggende SharePoint-websted. Microsoft arbejder på en rettelse. I mellemtiden kan du bruge følgende løsninger til at slette den private kanal.

**Udelad gruppe-eller gruppe af websteder fra SharePoint-opbevaringspolitikken.**

1. Gå til Office 365 administrations portalen, og vælg **Vis alle** i venstre navigationsrude.
2. Gå **Admin centers**til **Security &**  >  politik for**forebyggelse af datatab**under administration  >  **Policy**.
3. Identificer alle politikker, der gælder for SharePoint-websteder, og Rediger politikken, så SharePoint-webstedet for det team, der indeholder den private kanal, ikke er omfattet af opbevaringspolitikken.
4. Gem politikken.
    Det kan tage op til 24 timer, før politikindstillingerne træder i kraft.
    Når webstedet er blevet udeladt, kan du slette den private kanal.  
    
Du vil  ***muligvis*** kunne slette den private kanal ved hjælp af Microsoft teams på din Android-enhed. 

Hvis du vil have relaterede SharePoint-oplysninger, skal du se [kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).