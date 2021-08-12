---
title: Følsomhedsmærkater vises ikke
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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061426"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomhedsmærkater vises ikke

Følsomhedsmærkater giver dig mulighed for at klassificere og beskytte dit følsomme indhold. De kan oprettes i Microsoft 365 Overholdelsescenter, Microsoft 365 sikkerhedscenter eller Microsoft 365 & Compliance Center under Klassificering > Følsomhedsmærkater. Du kan få mere at vide om denne funktion [under Oversigt over følsomhedsmærkater.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Hvis du har konfigureret dine følsomhedsmærkater, men de ikke vises i Microsoft 365 apps, skal du kontrollere følgende:

- Bekræft, at følsomhedsmærkatet [er](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) blevet publiceret for de brugere og grupper, du ønsker.

- Bekræft, at brugeren bruger en app, der understøtter følsomhedsmærkater – [se følsomhedsmærkaterne i dit dokument.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Hvis du overfører Azure [Information Protection-etiketter, skal](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)du være opmærksom på de overvejelser, der er angivet [her.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Understøttelse af forebyggelse af datatab (DLP): I øjeblikket kan kun opbevaringsetiketter bruges som en betingelse i DLP-politikker.  Understøttelse af følsomhedsmærkater i en DLP-politik er ikke tilgængelig endnu, men vi arbejder på det.

- Når kryptering er aktiveret på et følsomhedsmærkat, kan du vælge enten at:
    - Tildel tilladelser nu
    - Lad brugere tildele tilladelser


Du kan finde flere oplysninger om mulige problemer under [Kendte problemer med følsomhedsmærkater.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)