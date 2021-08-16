---
title: Ret forbindelsespolitik
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988083"
---
# <a name="fix-connection-policy"></a>Ret forbindelsespolitik

Mailen blev markeret som sikker og leveret til brugerens indbakke, fordi den afsendende IP-adresse er markeret som sikker i politikken forbindelsesfilter. Hvis du vil gennemse politikken, skal du gøre følgende:

1. Gå til Office 365 [Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå derefter til   >    >  [Antispampolitik for trusselsstyring](https://go.microsoft.com/fwlink/?linkid=2101518).
2. På fanen **Brugerdefineret** skal du vælge **filterpolitikken Forbindelse** og derefter vælge **Rediger politik**.
3. Gennemse **listen over tilladte IP-adresser.** Se, **Pengeskab listen** er aktiveret.

    > [!NOTE]
    > Microsoft abonnerer på tredjepartskilder for afsendere, der er tillid til. Hvis **Pengeskab liste er** aktiveret, markeres disse afsendere, der er tillid til, ikke ved en fejltagelse som spam. Jeg anbefaler, at du vælger denne indstilling, da det vil reducere antallet af falske positive (gode mails, der er klassificeret som spam), som du modtager.
