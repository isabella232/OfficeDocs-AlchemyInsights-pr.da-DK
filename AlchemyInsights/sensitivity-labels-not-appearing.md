---
title: Følsomheds mærkater vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801178"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomheds mærkater vises ikke

Med følsomheds navne kan du klassificere og beskytte dit følsomme indhold. De kan oprettes i Microsoft 365 Compliance Center, Microsoft 365 Security Center eller Microsoft 365 Security & Compliance Center under klassificering > følsomheds mærkater. Hvis du vil have mere at vide om denne funktion, skal du se [Oversigt over følsomheds navne](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Hvis du har konfigureret dine følsomheds mærkater, men de ikke vises i Microsoft 365-apps, skal du kontrollere følgende:

- Bekræft, at følsomheds navnet er blevet [publiceret](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) til de brugere og grupper, du vil bruge.

- Bekræft, at brugeren bruger en app, der understøtter følsomheds mærkater – Se [følsomheds mærkater i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Hvis du over [fører Azure information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), skal du være opmærksom på de overvejelser, der er angivet [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Support til forebyggelse af datatab (DLP): i øjeblikket er det kun opbevarings etiketter, der kan bruges som en betingelse i DLP-politikker.  Understøttelse af følsomheds mærkater i en DLP-politik er ikke tilgængelig endnu, men vi arbejder på det.

- Når kryptering er aktiveret på en følsom etiket, kan du vælge enten at:
    - Tildel tilladelser nu
    - Lade brugere tildele tilladelser


Hvis du vil have mere at vide om mulige problemer, skal du se [kendte problemer med følsomheds navne](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).