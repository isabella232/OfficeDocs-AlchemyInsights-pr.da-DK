---
title: Følsomheds etiketter vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048646"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomheds etiketter vises ikke

Med følsomheds etiketter kan du klassificere og beskytte dit følsomme indhold. De kan oprettes i Microsoft 365 Compliance Center, Microsoft 365 Security Center eller Office 365 Security & Compliance Center underklassifikation > følsomheds etiketter. Du kan få mere at vide om denne funktion i [Oversigt overfølsomheds etiketter](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Hvis du har konfigureret dine følsomheds etiketter, men de ikke vises i Office-Apps, skal du kontrollere følgende:

- Bekræft, at følsomheds etiketten er blevet [publiceret](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) til de brugere og grupper, du ønsker.

- Bekræft, at brugeren bruger en app, der understøtter følsomheds etiketter – Se [følsomheds etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Hvis du [migrerer Azure information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), skal du være opmærksom på de overvejelser, der er anført [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Understøttelse af forhindring af datatab (DLP): i øjeblikket kan kun opbevarings etiketter bruges som en betingelse i DLP-politikker.  Understøttelse af følsomheds etiketter i en DLP-politik er endnu ikke tilgængelig, men vi arbejder på den.

- Når kryptering er aktiveret på en følsomheds etiket, kan du vælge enten at:
    - Tildel tilladelser nu
    - Lade brugere tildele tilladelser


Du finder flere oplysninger om mulige problemer under [kendte problemer med følsomheds etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).