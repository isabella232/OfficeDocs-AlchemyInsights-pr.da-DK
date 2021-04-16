---
title: Når du dobbeltklikker på en Office-fil, åbnes den ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814799"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Når du dobbeltklikker på en Office-fil, åbnes den ikke

Når du dobbeltklikker på en Office-fil, kan du se programmet åbne, men selve filen åbnes ikke. Eller du får muligvis fejlen: "Der opstod et problem med at sende kommandoen til programmet." Der er mange årsager til dette, men de to mest almindelige løsninger er:

- I Excel skal du sikre dig, at DDE-indstillingen ikke er markeret. Indstillingen kan findes ved at oprette en ny projektmappe og derefter vælge Filer **> Indstillinger > Avanceret**. I sektionen **Generelt skal** du fjerne markeringen i **Ignorer andre programmer, der bruger Dynamic Data Exchange (DDE).**

- Kør en onlinereparation for at gendanne standardindstillingerne. Klik på knappen Start i Windows, og søg efter "Kontrolpanel". Åbn **Kontrolpanel ,** og gå til **Programmer > Programmer og funktioner**. Højreklik derefter på **Microsoft Office [Version], og** vælg Skift > **Onlinereparation**.

Hvis ingen af disse løsninger virker, kan du finde en mere komplet liste over løsninger i supportartikel, hvor du ikke kan åbne [en Office-fil ved at dobbeltklikke på den.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
