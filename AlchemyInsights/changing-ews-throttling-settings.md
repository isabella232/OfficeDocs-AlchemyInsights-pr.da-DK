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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968371"
---
# <a name="changing-ews-throttling-settings"></a>Ændring af EWS-begrænsningsindstillinger

Kør vores automatiserede test, som giver dig mulighed for at ændre EWS-begrænsningspolitikken, så længe overførslen varer. Bemærk, at selv efter denne kørsel vil EWS-importerne stadig være begrænset til 150 MB pr. 5 minutter pr. postkasse; For at opnå en højere overførselshastighed, skal du overføre flere brugere samtidigt.

Bemærk, at ændringer i EWS-begrænsningspolitikken ikke har nogen indflydelse på følgende overførselstyper (ved hjælp af Microsoft-værktøjer): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Offentlig mappe eller PST-importtjeneste.