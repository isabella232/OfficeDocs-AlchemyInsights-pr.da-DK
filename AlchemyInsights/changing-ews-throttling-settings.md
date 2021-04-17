---
title: Ændring af EWS-begrænsningsindstillinger
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818030"
---
# <a name="changing-ews-throttling-settings"></a>Ændring af EWS-begrænsningsindstillinger

Kør vores automatiserede test, som giver dig mulighed for at ændre EWS-begrænsningspolitikken, så længe overførslen varer. Bemærk, at selv efter denne kørsel vil EWS-importerne stadig være begrænset til 150 MB pr. 5 minutter pr. postkasse; For at opnå en højere overførselshastighed, skal du overføre flere brugere samtidigt.

Bemærk, at ændringer i EWS-begrænsningspolitikken ikke har nogen indflydelse på følgende overførselstyper (ved hjælp af Microsoft-værktøjer): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Offentlig mappe eller PST-importtjeneste.