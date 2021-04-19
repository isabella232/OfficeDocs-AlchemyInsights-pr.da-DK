---
title: Der mangler Configuration Manager-enheder i portalen
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
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817238"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Der mangler Configuration Manager-enheder i portalen

For at enhedssynkronisering kan fungere, skal du [nødvendige internetslutpunkter](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) kunne nås fra den lokale server, der hoster rollen Tjenesteforbindelsespunkt. Hvis du vil foretage fejlfinding af enhedssynkronisering, skal du se **CMGatewaySyncUploadWorker.log**, der er placeret på tjenesteforbindelsespunktet.

Få mere at vide om [Tilknytning af lejer i Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
