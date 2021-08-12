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
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944125"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemer med at bruge Intune-administrationskonsollen

**"Adgang nægtet" når du navigerer i Intune-administrationsportalen.**

- Hvis du er medlem af en brugerdefineret Intune-rolle, skal du sikre dig, at der er tildelt en Intune- eller Enterprise Mobility Suite (EMS)-licens til din konto.
- Hvis du bruger en Konfigurationsstyring administrere enheder, skal du kontrollere, at du ikke er en del af Intune-brugersamlingen for Konfigurationsstyring MDM.
- Kontrollér, at du har fået tildelt de relevante rollebaserede tilladelser for administrationskontrol (RBAC) i intune-rollebladet.
- Kontrollér, at den anvendte gruppe ikke er en distributionsliste. Intune i Azure-portalen understøtter kun brugerkonti, der tilhører Azure Active Directory sikkerhedsgrupper. Gennemse dine grupper på Azure-portalen > **Intune-grupper**  >  eller i Azure-portalen > **Azure Active Directory**.

**Brugeren har for mange tilladelser til tildelt Intune-rolle**

Få brugeren til at gå til **Intune**  >  **Intune-roller**  >  **Mine eksporttilladelser** for at gennemse tildelte  >   tilladelser.

**Jeg har føjet en områdegruppe til en rolle, men brugere i den pågældende rolle kan stadig se andre brugere eller enheder.**

Omfangsgrupper filtrerer ikke brugere eller enheder fra. Omfangsgrupper:

- Begræns, hvem brugere kan tildele politikker eller programmer til.
- Tillad kun bestemte brugere at køre fjernopgaver på enheder.

Du kan finde flere oplysninger om [omfangsgrupper under Rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Jeg har føjet en bruger til en Intune-rolle, men de har stadig fuld adgang til Intune-administrationskonsollen.**

Gå til Intune **>-brugere** i Azure-portalen, og bekræft, at brugeren ikke er tildelt nogen af følgende roller i Azure-portalen:

- Global administrator
- Intune-tjenesteadministrator
- SharePoint administrator

Du kan finde flere [oplysninger i Rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemer med adgang**

Du kan få mere [at vide under Du kan ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).