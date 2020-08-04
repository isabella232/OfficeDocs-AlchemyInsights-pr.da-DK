---
title: Problemer med at bruge Intune-administrationskonsollen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554882"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemer med at bruge Intune-administrationskonsollen

**"Adgang nægtet", når du navigerer i Intune-administrationsportalen.**

- Hvis du er medlem af en brugerdefineret Intune-rolle, skal du sikre dig, at der er tildelt en INtune- eller Enterprise Mobility Suite-licens (EMS) til din konto.
- Hvis du bruger Konfigurationsstyring til at administrere enheder, skal du kontrollere, at du ikke er en del af Intune-brugersamlingen for Configuration Manager MDM.
- Kontroller, at du har fået tildelt de relevante rollebaserede rbac-tilladelser (Role-based Administration Control) i bladet Intune-roller.
- Kontroller, at den anvendte gruppe ikke er en distributionsliste. Intune på Azure-portalen understøtter kun brugerkonti, der tilhører Azure Active Directory-sikkerhedsgrupper. Gennemse dine grupper i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.

**Brugeren har for mange tilladelser til tildelt intune-rollen**

Råd til brugeren om at gå **til Intune**  >  **Intune-roller Mine**tilladelser  >  **My permissions**  >  **Eksporter for** at gennemse tildelte tilladelser.

**Jeg har føjet en områdegruppe til en rolle, men brugere i den rolle kan stadig se andre brugere eller enheder.**

Områdegrupper bortfiltrer ikke brugere eller enheder. Områdegrupper:

- Begræns, hvem brugere kan tildele politikker eller programmer til.
- Tillad kun bestemte brugere at køre fjernopgaver på enheder.

Yderligere oplysninger om områdegrupper finder du [i Role-based access control (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Jeg har føjet en bruger til en Intune-rolle, men de har stadig fuld adgang til Intune-administrationskonsollen.**

Gå til Intune > **Brugere** i Azure-portalen, og kontroller, at brugeren ikke er tildelt nogen af følgende roller på Azure-portalen:

- Global administrator
- Intune-tjenesteadministrator
- SharePoint-administrator

Yderligere oplysninger finder du [i Role-based access control (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemer med adgang**

Du kan finde flere oplysninger [under Du kan ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).