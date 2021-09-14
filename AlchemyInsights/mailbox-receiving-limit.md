---
title: Håndhævelse af begrænsning for postkasse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315834"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Håndhævelse af begrænsning for postkasse

Microsoft er for nylig begyndt at håndhæve grænsen pr. postkasse på 3600 meddelelser pr. time. Du kan finde flere oplysninger [Exchange Online begrænsninger](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 postkasser, der modtager mere end 3600 meddelelser inden for en time, bliver begrænseret i de næste 60 min. 

Desuden er grænsen for afsender-modtager-par, der blokerer meddelelser, der modtages af en Microsoft 365-postkasse fra en bestemt afsender, anvendt. Hvis en enkelt afsender sender over 33 % af den samlede grænseværdi eller 1200 meddelelser pr. rullende time til en bestemt modtager, kickstarter SRP-grænsen, og postkassen accepterer ikke længere meddelelser fra den pågældende afsender. Bemærk, at:

- Denne grænse gælder for mails, der modtages fra andre lejere, lokale afsendere eller internetafsendere.
- Levering af mail til postkassen blokeres i de næste 60 minutter. 
- Afsendere til disse postkasser modtager en rapport om manglende levering (5.2.121 eller 5.2.122) om, at postkassen har overskredet den maksimale grænse for levering. Intra-tenant (mail i samme lejer) leveres fortsat.
- Når SRP-grænsen er anvendt, fortsætter den modtagende postkasse med at acceptere meddelelser fra andre afsendere.

Administratorer kan overvåge aktuel postkasseaktivitet ved at få adgang til en ny rapport og indsigt i Exchange Administration kaldet "Postkasser, der overskrider modtagegrænser." Indsigten vises kun, hvis en lejer har stødende postkasser, mens rapporten altid vises på dashboardet, men er tom, medmindre en lejer har stødende postkasser.

Du kan få mere at vide om indsigt, der modtager begrænsninger, under Postkasser, der overskrider indsigt [i begrænsninger i det nye EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Du kan finde flere oplysninger om, hvordan du overskrider den rapport om begrænsninger, der modtages, under Postkasser, der overskrider den modtagende [grænserapport i den nye rapport om begrænsninger for modtager ( EAC).](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)