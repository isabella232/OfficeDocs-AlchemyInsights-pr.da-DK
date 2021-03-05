---
title: Klargøring af arbejdsdag til AD-bruger går i karantænetilstand
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481096"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Klargøring af arbejdsdag til AD-bruger går i karantænetilstand

**Klargøring af arbejdsdag til AD-bruger går i karantænetilstand, og der oprettes ingen brugere i AD**

Klargøringsjobbet Arbejdsdag til AD-bruger er gået i karantæne, og overvågningsloggen viser eksportfejlhændelser med fejlmeddelelsen **Fejl: OperationsError-SvcErr: Der opstod en handlingsfejl. Der er ikke konfigureret nogen overordnet reference for katalogtjenesten. Katalogtjenesten kan derfor ikke udstede henvisninger til objekter uden for denne skov.** Denne fejl vises normalt, hvis Active Directory Container OU ikke er angivet korrekt, eller hvis der er problemer med Udtrykstilknytning, der bruges til **parentDistinguishedName.**

Kontrollér, om der er slåfejl i **standardparameteren** OU for nye brugere. Kontrollér, at den angivne OU allerede findes i din AD. Hvis du bruger **parentDistinguishedName** i attributtilknytningen, skal du sikre dig, at den altid evalueres til en kendt beholder inden for AD-domænet. Kontrollér eksporthændelsen i overvågningslogfilerne for at få vist den genererede værdi.

Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk klargøring af brugere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

