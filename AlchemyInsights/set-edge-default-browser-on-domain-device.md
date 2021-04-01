---
title: Angiv Microsoft Edge som standardbrowser på en domæneforenet enhed
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491441"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Angiv Microsoft Edge som standardbrowser på en domæneforenet enhed

Angiv Microsoft Edge som standardbrowser: 

1. [Opret en standardtilknytninger for](https://go.microsoft.com/fwlink/?linkid=2132437) konfigurationsfilen, og gem den lokalt eller på et netværksshare.

1. Åbn editoren Gruppepolitik, og gå derefter til Administrative skabeloner til  >  **computerkonfiguration,**  >  **Windows Components**  >  **Stifinder.**

1. Vælg **Angiv en standard tilknytninger til konfigurationsfil.**

1. Vælg **Politikindstilling,** og vælg derefter **Aktiveret.**

1. Under **Indstillinger** skal du angive placeringen af standard tilknytninger til konfigurationsfilen og derefter vælge **OK.**
