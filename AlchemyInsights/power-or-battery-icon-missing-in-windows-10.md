---
title: Strøm- eller batteriikon mangler i Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790542"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Strøm- eller batteriikon mangler i Windows 10

Hvis din Windows 10-enhed har et batteri (f.eks. bærbar computer eller tablet eller en pc, der er sluttet via USB til en UPS), vises der normalt et strøm/batteriikon på proceslinjen i nærheden af uret, f.eks.:

![Batteriikon](media/battery-icon.png)

Hvis du ikke kan se dette ikon, kan det være skjult:

1. Gå til **[Indstillinger > Personlig tilpasning > proceslinjen.](ms-settings:taskbar?activationSource=GetHelp)**

2. I meddelelsesområdet skal du klikke på **Vælg, hvilke ikoner der skal vises på proceslinjen.**

3. Find **power-elementet** på listen, og skift indstillingen til **Til**.

    ![Vis power-ikon på proceslinjen](media/power-icon-on.png)

**Fejlfinding**

Hvis du har fulgt vejledningen ovenfor, og til/fra-knappen Tænd/slud er nedtonet eller  ikke synlig, skal du skrive Enhedshåndtering i søgefeltet på proceslinjen og derefter vælge Enhedshåndtering på listen over resultater.  Under **Batterier skal** du højreklikke på batteriet til din enhed, klikke på **Deaktiver** og klikke på **Ja**. Vent et par sekunder, og højreklik derefter på batteriet, og klik på **Aktivér.** Genstart derefter enheden.

Hvis du har fulgt vejledningen ovenfor, men batteriikonet ikke vises på proceslinjen, skal du skrive  Jobliste i søgefeltet på proceslinjen og derefter klikke på Jobliste på listen over resultater. På fanen **Processer** under Navn skal **du** højreklikke på **Stifinder** og derefter klikke på **Genstart.**
