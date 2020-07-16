---
title: Problem med at åbne eller hente filer i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148205"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem med at åbne eller hente filer i Yammer

Klassisk Yammer understøtter flere muligheder for filoverførsler til meddelelser og grupper. Afhængigt af netværkskonfigurationen er filerne som standard lager i SharePoint.

Filvælgeren i den nye Yammer understøtter endnu ikke alle de muligheder, der er tilgængelige i klassisk Yammer. En fremtidig opdatering vil tilføje yderligere funktioner. Du kan finde flere oplysninger [under Vedhæfte en fil eller et billede til et Yammer-samtaleindlæg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**En fil kan ikke åbnes eller hentes**  

En fil overføres muligvis til Yammer, men linker også til en fil i SharePoint Online. Hvis du vil foretage fejlfinding, skal du først bestemme filens placering. Hvis filen er blevet overført til Yammer, har den en *.yammer.com URL-adresse. Sørg for, at påkrævede URL-adresser og IP-adresser er fjernet. Du kan finde flere oplysninger i blogindlægget [Brug af hårde kodede IP-adresser til Yammer anbefales ikke](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Kontroller, om en bruger, der også er global administrator, kan hente filen. Hvis filen er privat, skal du muligvis bruge Privat indholdstilstand. Du kan finde flere oplysninger under [Overvåge privat indhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gæster og filer på Yammer-netværksniveau i SharePoint Online**  

[Gæster på netværksniveau i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruger ikke Azure AD B2B og er interne i Yammer-tjenesten, så de kan ikke få adgang til Yammer-filer, der er gemt i SharePoint. Opret en ekstern AAD B2B-bruger, der kan få adgang til dokumentbiblioteker i SharePoint Online ved hjælp af denne identitet. Du kan finde oplysninger om fremtidig Azure AD B2B-gæstesupport i Yammer under [Support af gæster i Business-to-business (B2B) i Yammer Preview – Kundevilkår og ofte stillede spørgsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).