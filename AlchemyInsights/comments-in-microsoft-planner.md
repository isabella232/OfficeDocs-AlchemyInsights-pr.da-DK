---
title: Kommentarer i Microsoft Planner
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
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817634"
---
# <a name="comments-in-microsoft-planner"></a>Kommentarer i Microsoft Planner

Opgavekommentarer i en plan er gemt i Exchange Online-postkassen for den Microsoft 365-gruppe, der er knyttet til planen.  Når du skriver en kommentar til en opgave, sendes der en mail til gruppens indbakke, og du modtager en mail for hver kommentar, der efterfølgende skrives på den pågældende opgave.

Her er nogle svar på almindelige problemer, der er relateret til kommentarer:

- **Brugere modtager ikke mails** – kommentarer sendes til gruppens indbakke for den gruppe, som planen tilhører. Hvis en bruger skal modtage gruppe mails, skal gruppen være konfigureret til at sende gruppesamtaler til medlemmets indbakker.

- **Kommentarer gemmes ikke** – Brugeren, der tilføjer kommentaren, har ikke tilladelse til at sende mails til Microsoft 365-gruppen. Læs [Sådan fungerer Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for at få mere at vide om dette scenarie.

- Fejlen **Du har ikke længere adgang** vises, eller **gæstebrugere kan ikke tilføje kommentarer** – gæstebrugere, der ikke kan sende en mail til gruppens indbakke, får muligvis vist denne meddelelse. Du kan løse dette problem ved at sikre, at gæstebrugeren har en gyldig mailadresse.

- **Fjernede brugere får mails** – hvis en bruger kommenterer på en opgave, før den fjernes fra planen, medtager mailtråden brugeren til hver kommentar, der skrives på opgaven.

Hvis du vil have mere at vide om kommentarer med Microsoft Planner, kan du se [Sådan fungerer Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) og [Skriv en kommentar til opgaver i Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
