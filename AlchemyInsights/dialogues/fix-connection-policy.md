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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693300"
---
# <a name="fix-connection-policy"></a>Ret forbindelsespolitik

Mailen blev markeret som sikker og leveret til brugerens indbakke, fordi den afsendende IP-adresse var markeret som sikker i politikken Forbindelsesfilter. Hvis du vil gennemse politikken, skal du gøre følgende:

1. Gå til [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå derefter **til** antispam  >  **for politikker**  >  [for trusselsadministration.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Vælg **filterpolitikken** Forbindelse under fanen **Brugerdefineret, og** vælg derefter **Rediger politik.**
3. Gennemse **listen over tilladte IP-adresser.** Se, om **listen over sikre personer** er aktiveret.

    > [!NOTE]
    > Microsoft abonnerer på tredjepartskilder for afsendere, der er tillid til. Hvis **listen er** aktiveret, markeres disse afsendere, der er tillid til, ikke ved en fejltagelse som spam. Jeg anbefaler at vælge denne indstilling, da det vil reducere antallet af falske positive (gode mails, der er klassificeret som spam), som du modtager.
