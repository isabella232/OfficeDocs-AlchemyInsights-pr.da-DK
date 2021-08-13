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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966103"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Der mangler Configuration Manager-enheder i portalen

For at enhedssynkronisering kan fungere, skal du [nødvendige internetslutpunkter](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) kunne nås fra den lokale server, der hoster rollen Tjenesteforbindelsespunkt. Hvis du vil foretage fejlfinding af enhedssynkronisering, skal du se **CMGatewaySyncUploadWorker.log**, der er placeret på tjenesteforbindelsespunktet.

Få mere at vide om [Tilknytning af lejer i Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
