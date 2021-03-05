---
title: Problem med attribut og angivelse af filter
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481100"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem med attribut og angivelse af filter

**Problem med modstridende UPN-værdier**

The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Handlingen mislykkedes, fordi UPN-værdien, der er angivet til tilføjelse/ændring, ikke er entydig for hele skoven. Fejldetaljer: **CONSTRAINT_ATT_TYPE – userPrincipalName.**

**UserPrincipalName-værdien,** som Forbindelseskomponent Arbejdsdag forsøger at angive, når du opretter AD-brugerkontoen, findes allerede i AD-destinationsdomænet. Dette antyder, at enten (1) brugeren allerede findes, og den matchende id-kontrol mislykkedes for brugeren, eller (2) upn-generationreglen genererede en modstridende værdi.

Her er de foreslåede trin til løsning:

Hvis brugeren allerede findes, og den matchende id-kontrol ikke kunne sammenkæde arbejdsdagskontoen med Active Directory-kontoen, skal du kontrollere, om den matchende id-attribut (typisk medarbejder-id) i både Arbejdsdag og AD har et nøjagtigt match. Hvis de ikke har et match, er det et dataproblem, der skal rettes. Hvis medarbejder-id'et i arbejdsdagen f.eks. er 001052, og i AD er det 1052, så kan klargøringsprogrammet ikke sammenkæde de to konti og forsøger at oprette en bruger, der allerede findes. Løsningen i dette tilfælde er at ændre værdien for **Medarbejder-id** i AD, så den medtager de foranstillede nuller for at gøre den til 001052.
Hvis det UPN-genererende udtryk ikke genererer en entydig værdi, kan du overveje at bruge duplikeringsfunktionen **SelectUniqueValue** til at generere en entydig værdi hver gang.

**Arbejdsdag til AD-bruger klargøring angiver ikke administratorattributværdien for AD-brugerkonto**

Jobbet til klargøring af arbejdsdag til AD-bruger angiver ikke **administratorattributværdien** for AD-brugerkonti. Der er to mulige scenarier, når denne funktionsmåde kan ses:

1. Chefen i Arbejdsdag kan ikke løses til en tilsvarende AD-brugerkonto, fordi lederen ikke er omfattet.
2. I et **scenarie med flere AD-domæner** er chefen i Arbejdsdag ikke til stede i det samme domæne som brugeren.

Prøv disse trin for at løse problemet:

1. Hvis du har defineret områdefiltre, skal du først kontrollere, om den overordnede er i omfang, og at den opfylder angivelsessætningen. Hvis lederen ikke opfylder filterets område, skal du ændre filteret, så lederen også er i forbindelse med klargøringshandlingen.
2. Hvis du har flere AD-domæner, har forbindelsen en kendt begrænsning for manglende mulighed for at løse referencer til administration på tværs af domæner.

Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk klargøring af brugere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













