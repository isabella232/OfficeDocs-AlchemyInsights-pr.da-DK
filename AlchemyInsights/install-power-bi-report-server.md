---
title: Installere Power BI Report Server
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
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832088"
---
# <a name="install-power-bi-report-server"></a>Installere Power BI Report Server

1. Find placeringen af PowerBIReportServer.exe og start installationsprogrammet.

2. Vælg **Installer Power BI Report Server**.

3. Vælg en udgave, der skal installeres, og vælg **derefter Næste**.

4. Du kan vælge enten Evaluation eller Developer på rullelisten.  Ellers kan du angive en produktnøgle til den server, du har købt fra enten Power BI-tjenesten eller Volume License Service Center. Du kan finde flere oplysninger om, hvordan du får din produktnøgle, i afsnittet Før du begynder. Læs og agree to the license terms and conditions, and then select **Next**.

5. Du skal have et databaseprogram tilgængeligt for at gemme rapportserverdatabasen. Vælg **Næste** for kun at installere rapportserveren.

6. Angiv installationsplaceringen for rapportserveren. Vælg **Installer for** at fortsætte.

7. Efter korrekt konfiguration skal du vælge **Konfigurer rapportserver for** at starte Reporting Services Konfigurationsstyring.

Du behøver ikke en SQL Server Database Engine-server, der er tilgængelig på installations tidspunkt. Du skal bruge en til at konfigurere Reporting Services efter installationen.

Du kan finde flere oplysninger: https://docs.microsoft.com/power-bi/report-server/install-report-server
