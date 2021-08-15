---
title: Der kan ikke logges Teams på grund af fejl autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038394"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Der kan ikke logges Teams på grund af fejlen autologon.microsoftazuread-sso dot com:443

Hvis Seamless SSO er aktiveret som O365-godkendelse, skal URL-autologon.microsoftazuread-sso.com muligvis føjes til intranetwebsteder.  Hvis den tidligere er blevet føjet til Pålidelige websteder, og Seamless SSO er i brug, bør den fjernes fra Websteder, du har tillid til.

Gennemgå Tjekliste [til fejlfinding af enkelt brugers enkeltliste til problemfri sso.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)

Følg disse trin for at føje en URL-adresse til listen Intranetwebsteder:

1. Åbn Internet Explorer ved at klikke på **knappen** Start. Skriv Internet Explorer i søgefeltet, og klik derefter på Internet Explorer på listen over **resultater.**
2. Klik **på Værktøjer**, og klik derefter på **Internetindstillinger**.
3. Klik på **fanen** Sikkerhed.
4. Klik nu på **Lokale intranetwebsteder,** og klik derefter på **knappen Websteder** og derefter på **knappen** Avanceret.
5. Angiv webstedets URL-adresse, og klik **på Tilføj**.
6. Når du er færdig, skal du klikke **på Luk**.

Du kan finde flere oplysninger i Dokumentation til installation af Seamless SSO til [O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (omfatter politikbaseret proces til at tilføje en URL-adresse til intranetwebsteder i trin 3).
