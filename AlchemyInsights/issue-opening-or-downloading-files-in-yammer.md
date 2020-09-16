---
title: Problem med at åbne eller hente filer i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695643"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem med at åbne eller hente filer i Yammer

Klassisk Yammer understøtter flere mulighederne for fil overførsler til meddelelser og grupper. Afhængigt af netværkskonfigurationen er filer som standard gemt i SharePoint.

Valg af fil i ny Yammer understøtter endnu ikke alle de muligheder, der er tilgængelige i klassisk Yammer. En fremtidig opdatering vil tilføje yderligere funktioner. Hvis du vil have mere at vide, skal du se [vedhæfte en fil eller et billede til et Yammer-samtale indlæg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Kan ikke åbne eller downloade en fil**  

En fil kan uploades til Yammer, men også oprette en kæde til en fil i SharePoint Online. For at foretage fejlfinding skal du først bestemme placeringen af filen. Hvis filen er blevet overført til Yammer, får den en *. yammer.com-URL-adresse. Kontrollér, at de påkrævede URL-adresser og IP-adresser ikke er blokeret. Hvis du vil have flere oplysninger, kan du se blogindlægget [ved hjælp af hard coded IP-adresser til Yammer](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Kontrollér, om en bruger, der også er en global administrator, kan downloade filen. Hvis filen er privat, skal du muligvis bruge privat indholds tilstand. Hvis du vil have mere at vide, skal du se [overvåge det private indhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gæster og filer i Yammer-netværksniveau i SharePoint Online**  

[Gæster på netværksniveau i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruger ikke Azure ad B2B og er interne for yammer-tjenesten, så de kan ikke få adgang til yammer-filer, der er gemt i SharePoint. Opret en ekstern AAD B2B-bruger, der kan få adgang til dokumentbiblioteker i SharePoint Online ved hjælp af den pågældende identitet. Hvis du vil have mere at vide om fremtidig Azure AD B2B-gæste support i Yammer, skal du se [gæste support i Business-to-business (B2B) i Yammer preview – kunde vilkår og ofte stillede spørgsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).