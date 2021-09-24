---
title: Skift fra Microsoft-navneservere tilbage til at administrere dine egne DNS-poster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506382"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Skift fra Microsoft-navneservere tilbage til at administrere dine egne DNS-poster

Du har tidligere ændret dine NS-poster til at pege på Microsoft (ns1.bdm.microsoftonline.com), men har nu besluttet at administrere dine egne DNS-poster:

På domæneregistratorens websted skal du ændre navneserveren tilbage til din registrator eller tidligere indstilling. Hvis du ikke kender DNS, skal du kontakte support hos domæneregistratoren. Bemærk, at det kan tage op til 48 timer, før navneserverændringerne er overført. 

1. I administrationsportalen Microsoft 365 skal du gå til **Indstillinger** Domæner , markere afkrydsningsfeltet ud for domænet  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)og vælge **DNS-styring**. 

2. Vælg Tilføj dine egne **DNS-poster i guiden,** og fuldfør guiden. Dette ændrer, hvordan din DNS administreres, og gør det derefter muligt at tilføje de brugerdefinerede DNS-poster, der skal bruges til at understøtte dine valgte tjenester.

Alternativt, Hvis du har ændret dine navneserverposter til Microsoft og har et websted, kan du tilføje DNS-poster for webstedet i stedet for at ændre navneserverne tilbage. Du kan få mere at vide [under Opdatere DNS-poster for at beholde dit websted hos din nuværende udbyder.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


