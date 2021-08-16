---
title: Installer Power BI-rapportserver
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
ms.openlocfilehash: 01cc2efc2dacc2fdf0b7b7f036bc18e1c75fd515348b72d5c4dde96949a51a2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028574"
---
# <a name="install-power-bi-report-server"></a>Installer Power BI-rapportserver

1. Find placeringen af PowerBIReportServer.exe og start installationsprogrammet.

2. Vælg **Installer Power BI-rapportserver**.

3. Vælg en udgave, der skal installeres, og vælg **derefter Næste**.

4. Du kan vælge enten Evaluation eller Developer på rullelisten.  Ellers kan du angive en produktnøgle til den server, du har købt hos enten Power BI-tjenesten eller Volume License Service Center. Du kan finde flere oplysninger om, hvordan du får din produktnøgle, i afsnittet Før du begynder. Læs og agree to the license terms and conditions, and then select **Next**.

5. Du skal have et databaseprogram tilgængeligt for at gemme rapportserverdatabasen. Vælg **Næste** for kun at installere rapportserveren.

6. Angiv installationsplaceringen for rapportserveren. Vælg **Installer for** at fortsætte.

7. Efter korrekt konfiguration skal du vælge **Konfigurer rapportserver for** at starte Reporting Services Konfigurationsstyring.

Du behøver ikke en SQL Server databaseprogramserver, der er tilgængelig på installations tidspunkt. Du skal bruge en til at konfigurere Reporting Services efter installationen.

Du kan finde flere oplysninger: https://docs.microsoft.com/power-bi/report-server/install-report-server
