---
title: Ændring af indstillinger for begrænsning af EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075891"
---
# <a name="changing-ews-throttling-settings"></a>Ændring af indstillinger for begrænsning af EWS

Kør vores automatiserede test, som giver dig mulighed for at ændre EWS-begrænsningspolitikken i hele overførslens varighed. Bemærk, at selv efter kørslen vil EWS-importerne stadig være begrænset til 150 mb pr. 5 minutter pr. postkasse. for at opnå højere overførselshastighed, skal du overføre flere brugere samtidigt.

Bemærk, at ændringer af EWS-begrænsningspolitikken ikke har nogen indflydelse på følgende overførselstyper (ved hjælp af Microsoft-værktøjer): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Offentlig mappe eller PST-importtjeneste.