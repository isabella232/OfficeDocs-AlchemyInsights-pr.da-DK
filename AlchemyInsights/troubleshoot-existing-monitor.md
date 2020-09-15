---
title: Fejlfinding af eksisterende skærm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690705"
---
# <a name="troubleshoot-an-existing-monitor"></a>Fejlfinding af en eksisterende skærm

Prøv disse løsninger for at foretage fejlfinding af en skærm. 

**Opdater skærmvisningen:**

Tryk på følgende taster på samme tid: Windows-tast + Ctrl + Skift + B. Dette vil opdatere kommunikationen med din grafikdriver. Dine skærme blinker kort øjeblik og vender tilbage efter et par sekunder.

**Fejlfinding på skærmhardware:**

1. Fjern kablet fra din PC til skærmen, og sæt den ind igen.
2. Fjern eventuelle ikke-vigtige enheder fra din PC (f. eks kort eller docker).

**Hvis du for nylig har installeret en opdatering på din PC, kan du vende tilbage til din skærmdriver:**

1. Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** fra resultaterne.
2. Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, ands Vælg **Egenskaber**.
3. Gå til fanen **driver** , og vælg **Annuller tilbage-driver**. <br>
Bemærk! Hvis den ikke er tilgængelig eller er nedtonet, skal du vælge **Nej** under nedenstående indstillinger for at gå til næste trin.
4. Du skal muligvis genstarte din PC, før ændringerne træder i kraft.

**Fjerne og geninstallere din skærmdriver:**

1. Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** fra resultaterne.
2. Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, ands Vælg **Fjern enhed**. 
3. Markér afkrydsningsfeltet ud for **Slet driversoftwaren til denne enhed** , og vælg **Fjern**.<br>
Bemærk! du bliver muligvis bedt om at genstarte computeren på dette tidspunkt. Husk at skrive de resterende instruktioner ned, før du genstarter.
4. Åbn Enhedshåndtering igen.
5. Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, og vælg **Opdater driver**.
6. Vælg **Søg automatisk efter Opdater driversoftware** , og følg installationsvejledningen.