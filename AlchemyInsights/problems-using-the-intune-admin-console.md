---
title: Problemer med at bruge Intune-administrationskonsollen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728281"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemer med at bruge Intune-administrationskonsollen

**"Adgang nægtet", når du navigerer til Intune-administrations portalen.**

- Hvis du er medlem af en brugerdefineret Intune-rolle, skal du sikre dig, at en Intune-eller Enterprise Mobility Suite-licens (EMS) er tildelt til din konto.
- Hvis du bruger Konfigurationsstyring til at administrere enheder, skal du kontrollere, at du ikke er en del af Intune-bruger samlingen for Configuration Manager MDM.
- Kontrollér, at du er blevet tildelt den relevante rollebaserede administrations kontrol (RBAC)-tilladelser i blade til Intune-roller.
- Kontrollér, at den anvendte gruppe ikke er en distributionsliste. Intune i Azure-portalen understøtter kun brugerkonti, der hører til Azure Active Directory-sikkerhedsgrupper. Gennemse dine grupper i Azure-portalen > **Intune**  >  -**grupper**eller i Azure-portalen > **Azure Active Directory**.

**Brugeren har for mange tilladelser til den tildelte Intune-rolle**

Adviser brugeren om at gå til **Intune**  >  **Intune-roller**  >  **mine tilladelser**  >  **eksport** for at gennemse de tilladelser, der er tildelt.

**Jeg har føjet en områdegruppe til en rolle, men brugere i den pågældende rolle stadig kan se andre brugere eller enheder.**

Områdegrupper filtrerer ikke brugere eller enheder. Områdegrupper:

- Begræns, hvem brugere kan tildele politikker eller programmer til.
- Tillad kun bestemte brugere at køre eksterne opgaver på enheder.

Du kan finde flere oplysninger om områdegrupper under  [rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Jeg har føjet en bruger til en Intune-rolle, men de har stadig fuld adgang til Intune-administrationskonsollen.**

Naviger til Intune > **brugere** i Azure-portalen, og kontrollér, at brugeren ikke er tildelt en af følgende roller i Azure-portalen:

- Global administrator
- Intune-tjenesteadministrator
- SharePoint-administrator

Du kan finde flere oplysninger under [rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Adgangsproblemer**

Du kan finde flere oplysninger i [kan du ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).