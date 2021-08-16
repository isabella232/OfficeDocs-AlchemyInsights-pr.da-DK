---
title: Problem med at åbne eller downloade filer i Yammer
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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028244"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem med at åbne eller downloade filer i Yammer

Klassisk Yammer understøtter flere muligheder for filoverførsler til meddelelser og grupper. Afhængigt af netværkskonfigurationen gemmes filerne som standard i SharePoint.

Filvælgeren i den nye Yammer understøtter endnu ikke alle de muligheder, der er tilgængelige i den klassiske Yammer. En fremtidig opdatering vil tilføje yderligere funktioner. Få mere at vide under [Vedhæft en fil eller et billede i et Yammer samtaleindlæg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Det er ikke muligt at åbne eller downloade en fil**  

En fil kan blive overført til Yammer men også oprette et link til en fil SharePoint Online. Hvis du vil foretage fejlfinding, skal du først bestemme placeringen af filen. Hvis filen er blevet overført til Yammer, har den en *.yammer.com URL-adresse. Sørg for, at nødvendige URL-adresser og IP-adresser ikke er blokerede. Du kan finde flere oplysninger i [blogindlægget Brug af hard coded IP-adresser Yammer ikke anbefales.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Kontrollér, om en bruger, som også er global administrator, kan hente filen. Hvis filen er privat, skal du muligvis bruge Privat indholdstilstand. Du kan få mere at vide under [Overvåge privat indhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer gæster og filer på netværksniveau i SharePoint Online**  

[Gæster på netværksniveau](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) i Yammer bruger ikke Azure AD B2B og er interne i Yammer-tjenesten, så de kan ikke få adgang til Yammer filer, der er gemt i SharePoint. Opret en ekstern AAD B2B-bruger, der har adgang til dokumentbiblioteker i SharePoint Online ved hjælp af den pågældende identitet. Hvis du vil have mere at vide om fremtidig Azure AD B2B-gæstesupport i Yammer, skal du se [B2B -gæstesupport (Business-to-business) i Yammer Preview –](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)kundevilkår og ofte stillede spørgsmål.