---
title: Ydelse af adgangs ydelser
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698676"
---
# <a name="access-services-retirement"></a>Ydelse af adgangs ydelser

Som vi oprindeligt har offentliggjort i MC97576, i marts 2017 og fortsat at kommunikere over de seneste års Access-tjenester udgår. Den næste fase i denne proces er at fjerne Access-webdatabaser, der bruger SharePoint-lister som underliggende datalager.

**Hvordan påvirker det mig?**

Fra juni 2019 stopper vi med at oprette nye Access-databaser i SharePoint Online og lukker tjenesten og eventuelle resterende apps ved april 2020.

**Hvad skal jeg gøre for at forberede denne ændring?**

Vi opfordrer dig til at oprette en overgangsplan for din organisations Access-webdatabaser. Administratorer kan bruge [Scannerprogrammet SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over de Access-apps, som websteder bruger.

Du kan overføre data fra Access-databaser på flere måder:

- Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette gratis virksomhedsløsninger til web-og mobilenheder.