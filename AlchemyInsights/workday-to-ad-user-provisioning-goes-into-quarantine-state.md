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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036486"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Klargøring af arbejdsdag til AD-bruger går i karantænetilstand

**Klargøring af arbejdsdag til AD-bruger går i karantænetilstand, og der oprettes ingen brugere i AD**

Klargøringsjobbet Arbejdsdag til AD-bruger er gået i karantæne, og overvågningslogfilerne viser eksportfejlhændelser med fejlmeddelelsen **Fejl: OperationsError-SvcErr: Der opstod en handlingsfejl. Der er ikke konfigureret nogen overordnet reference for katalogtjenesten. Katalogtjenesten kan derfor ikke udstede henvisninger til objekter uden for denne skov.** Denne fejl vises normalt, hvis Active Directory Container OU ikke er angivet korrekt, eller hvis der er problemer med udtrykstilknytning, der bruges til **parentDistinguishedName**.

Kontrollér standardparameteren OU for **nye brugere** for slåfejl. Kontrollér, at den angivne OU allerede findes i din AD. Hvis du bruger **parentDistinguishedName** i attributtilknytningen, skal du sikre dig, at den altid evalueres til en kendt beholder inden for AD-domænet. Kontrollér eksporthændelsen i overvågningslogfilerne for at få vist den genererede værdi.

Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk bruger klargøring](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

