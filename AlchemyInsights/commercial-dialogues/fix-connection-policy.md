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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314838"
---
# <a name="fix-connection-policy"></a>Ret forbindelsespolitik

Mailen blev markeret som sikker og leveret til brugerens Indbakke, fordi kilde-IP-adressen blev markeret som sikker i standardfilterpolitikken for forbindelse. Hvis du vil gennemse politikken, skal du gøre følgende:

1. I portalen Microsoft 365 Defender på skal du gå til & politikker for samarbejde & regler for trussel <https://security.microsoft.com/>  \>  \>  \> **mod spam** i **sektionen** Politikker.

   For at gå direkte til **siden Politikker for uønsket post** skal du bruge <https://security.microsoft.com/antispam> .

2. På siden **Politikker for uønsket post** skal du vælge politikken med navnet Forbindelsesfilterpolitik **(Standard)** ved at klikke på navnet på politikken.

3. I pop op-dialogboksen med oplysninger, der vises, **skal du klikke på Rediger** politik for filtrering af forbindelse i sektionen **Forbindelsesfiltrering.**

4. Gennemse posterne i afsnittet Tillad altid meddelelser fra følgende **IP-adresser** eller adresseområde, og se, om Aktiver **listen Over** sikre er markeret.

   **Bemærk!** Microsoft abonnerer på tredjepartskilder for afsendere, der er tillid til. Hvis listen over sikre afsendere er aktiveret, markeres disse afsendere, der er tillid til, ikke ved en fejltagelse som spam. Vi anbefaler, at du vælger denne indstilling, da det vil reducere antallet af falske positive (gode mails, der er klassificeret som spam), som du modtager.

Du kan finde flere oplysninger [under Konfigurere filtrering af forbindelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
