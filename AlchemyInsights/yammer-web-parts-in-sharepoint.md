---
title: Yammer-webdele i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664344"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Yammer-webdele i SharePoint

Yammer-samtaler og Yammer højlys fremhæver samarbejdet på moderne og klassiske SharePoint-sider. Du kan finde flere oplysninger i [yammer-samtaler](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  og Yammer-  [højlys](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).    

Webdelen moderne Yammer-samtaler opdateres til den nye Yammer-oplevelse og er tilgængelig for målrettede Release-lejere. GA-udrulning er startet. Nye funktioner omfatter muligheden for at starte en samtale med alle indlæg (spørgsmål, afstemninger, ros) og for at markere de bedste svar direkte fra SharePoint. Hvis du vil have mere at vide, skal du se [nye Yammer-kunde vilkår og ofte stillede spørgsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).

 Hvis du vil vide, hvilken webdel og konfiguration der passer til dig, skal du se [brug af en Yammer-webdel i SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).  

**Brug af webdele med SharePoint Server**  

Webdele kan bruges på moderne og klassiske sider i lokale miljøer.

- Du kan finde flere oplysninger om moderne sider under [føje et Yammer-feed til en moderne side i SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- Hvis du vil have mere at vide om klassiske sider, skal du se [føje et Yammer-feed til en klassisk side i SharePoint-servere 2013, 2016 og 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Yammer-integrering**  

Brug konfigurationsværktøjet Integrer til at teste Integrer forbrug. En fremtidig opdatering, der kan integreres, aktiverer den nye Yammer-oplevelse. Du kan finde flere oplysninger i [konfigurationsværktøjet til Yammer-integrering](https://aka.ms/YammerEmbedConfigureTool). Hvis du vil have mere at vide om Yammer-integrationskomponenten, skal du se [Integrer feed](https://aka.ms/YammerDevDocs).

**Kendte problemer og begrænsninger**

- Gruppe-ID'er er ikke tilgængelige fra nye Yammer URL-adresser, som er ændret. Skift tilbage til klassisk tilstand for at hente gruppe-id'er eller andre id'er fra URL-adresser.
- Brugerdefinerede domæner (Vanity) understøttes ikke.
- Yammer-integrering er ikke optimeret til mobil. Brug moderne sider med webdelen Yammer-samtaler for at få den bedste oplevelse.
- Brugerdefinerede temaer kan påvirke webdelen Yammer-samtaler, udseende og funktionalitet. Åbn en support situation for at rapportere problemer.