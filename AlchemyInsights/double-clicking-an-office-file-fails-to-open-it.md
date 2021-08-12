---
title: Når du dobbeltklikker på Office filen, åbnes den ikke
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
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965095"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Når du dobbeltklikker på Office filen, åbnes den ikke

Når du dobbeltklikker på Office fil, kan du muligvis se programmet åbne, men selve filen åbnes ikke. Eller du får muligvis fejlen: "Der opstod et problem med at sende kommandoen til programmet." Der er mange årsager til dette, men de to mest almindelige løsninger er:

- Sørg for, Excel DDE-indstillingen ikke er markeret, direkte fra feltet Indstillinger. Indstillingen kan findes ved at oprette en ny projektmappe og derefter vælge Filer **> Indstillinger > Avanceret**. I sektionen **Generelt** skal du fjerne markeringen i **Ignorer andre programmer, der bruger Dynamic Data Exchange (DDE).**

- Kør en onlinereparation for at gendanne standardindstillingerne. Klik på Windows Start, og søg efter "Kontrolpanel". Åbn **Kontrolpanel ,** og gå til **Programmer > Programmer og funktioner**. Højreklik derefter på Microsoft Office **[Version], og** vælg **Skift > Onlinereparation**.

Hvis ingen af disse løsninger virker, kan du finde en mere komplet liste over løsninger i supportartikel, hvor du ikke kan åbne [en Office-fil.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
