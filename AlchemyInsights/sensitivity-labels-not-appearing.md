---
title: Følsomhedsetiketter vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758383"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomhedsetiketter vises ikke

Følsomhedsetiketter giver dig mulighed for at klassificere og hjælpe med at beskytte dit følsomme indhold. De kan oprettes i Microsoft 365 compliance center, Microsoft 365 Security Center eller Microsoft 365 Security & Compliance Center under Klassifikation > Følsomhedsetiketter. Hvis du vil have mere at vide om denne funktion, skal du se [Oversigt over følsomhedsetiketter](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Hvis du har konfigureret dine følsomhedsetiketter, men de ikke vises i Office-apps, skal du kontrollere følgende:

- Bekræft, at følsomhedsetiketten [er](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) udgivet til de ønskede brugere og grupper.

- Bekræft, at brugeren bruger en app, der understøtter følsomhedsetiketter - se [følsomhedsetiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Hvis du [overfører Azure Information Protection-etiketter,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)skal du være opmærksom på de overvejelser, der er angivet [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Understøttelse af forebyggelse af datatab (DLP): I øjeblikket er det kun opbevaringsetiketter, der kan bruges som en betingelse i DLP-politikker.  Understøttelse af følsomhedsetiketter i en DLP-politik er endnu ikke tilgængelig, men vi arbejder på den.

- Når kryptering er aktiveret på en følsomhedsetiket, kan du vælge enten at:
    - Tildele tilladelser nu
    - Lad brugerne tildele tilladelser


Du kan finde flere oplysninger om mulige problemer under [Kendte problemer med følsomhedsetiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).