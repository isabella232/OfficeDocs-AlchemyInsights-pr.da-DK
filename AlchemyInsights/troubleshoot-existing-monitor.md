---
title: Fejlfinding af eksisterende skærm
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
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981071"
---
# <a name="troubleshoot-an-existing-monitor"></a>Fejlfinding af en eksisterende skærm

Prøv disse løsninger for at foretage fejlfinding af en skærm. 

**Opdater skærmens skærm:**

Tryk på følgende taster på samme tid: Windows-tasten + Ctrl + Skift + B. Dette opdaterer kommunikationen med grafikdriveren. Dine skærme blinker kortvarigt og vender tilbage efter et par sekunder.

**Fejlfinding af skærmhardware:**

1. Træk kablet ud, som forbinder pc'en med din skærm, og sæt det i igen.
2. Afbryd forbindelsen til alle ikke-vigtige enheder fra din pc (f.eks. adaptere eller docks).

**Hvis du for nylig har installeret en opdatering på din pc, kan du tilbagerulle skærmdriveren:**

1. Vælg **Start**, skriv **enhedshåndtering**, og **vælg Enhedshåndtering** fra resultaterne.
2. Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Egenskaber**.
3. Gå til fanen **Driver,** og vælg **Flyt driver tilbage.** <br>
Bemærk! Hvis dette ikke er tilgængeligt eller er nedtonet, skal du **vælge** Nej i indstillingerne nedenfor for at gå til næste trin.
4. Du skal muligvis genstarte computeren, før disse ændringer træder i kraft.

**Fjern og geninstaller skærmdriveren:**

1. Vælg **Start**, skriv **enhedshåndtering**, og **vælg Enhedshåndtering** fra resultaterne.
2. Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Fjern enhed**. 
3. Markér afkrydsningsfeltet ud for **Slet driversoftwaren til denne enhed, og** vælg **Fjern**.<br>
Bemærk! Du bliver muligvis bedt om at genstarte computeren på dette tidspunkt. Sørg for at skrive de resterende instruktioner ned, før du genstarter.
4. Åbn Enhedshåndtering igen.
5. Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Opdater driver.**
6. Vælg **Søg automatisk efter opdateringsdriversoftware,** og følg installationsvejledningen.