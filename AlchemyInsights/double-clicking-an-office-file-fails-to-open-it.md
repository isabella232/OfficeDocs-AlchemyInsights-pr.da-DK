---
title: Hvis du dobbeltklikker på en Office-fil, kan den ikke åbnes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573482"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Hvis du dobbeltklikker på en Office-fil, kan den ikke åbnes

Når du har dobbeltklikket på en Office-fil, kan du muligvis se, at programmet er åbent, men selve filen åbnes ikke. Eller du kan få fejlen: "Der opstod et problem under at sende kommandoen til programmet." Der er mange årsager til dette, men de to mest almindelige løsninger er:

- Fra Excel skal du sikre dig, at Indstillingen DDE ikke er markeret. Indstillingen kan findes ved at oprette en ny projektmappe og derefter vælge **Fil > Indstillinger > Avanceret**. Fjern markeringen i afkrydsningsfeltet **Ignorer andre programmer, der bruger DDE (Dynamic Data Exchange)** i sektionen **Generelt.**

- Kør en onlinereparation for at gendanne standardindstillingerne. Klik på knappen Start i Windows, og søg efter "Kontrolpanel". Åbn **Kontrolpanel**, og gå til **Programmer > Programmer og funktioner**. Højreklik derefter på **Microsoft Office [Version],** og vælg **Skift > Onlinerepair**.

Hvis ingen af disse løsninger fungerer, findes der en mere komplet liste over løsninger i supportartiklen, [dobbeltklik på en Office-fil kan ikke åbneden](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
