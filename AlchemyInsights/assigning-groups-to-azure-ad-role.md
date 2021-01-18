---
title: Tildele grupper til Azure AD-rolle
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884911"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tildele grupper til Azure AD-rolle

Hvis du vil tildele en Azure AD-gruppe med kilde til myndighed i Azure AD til en Azure AD-rolle, skal du udføre følgende trin:

1. Opret en ny gruppe – for at oprette en ny gruppe:

    a. Log på Azure AD administration med **privilegeret rolleadministrator** eller **globale administrator** tilladelser.
    b. Vælg **Azure Active Directory-> grupper > alle grupper > ny gruppe**.
    c. Opret gruppen.

2. Tildel gruppen rollen enten undergruppe oprettelse, eller efter at gruppen er oprettet.

    a. Hvis du vil tildele en rolle til gruppen på tidspunktet for gruppe oprettelsen, kan du skifte til til/fra- **roller i Azure ad, tildeles gruppen** og oprette gruppen.
    b. Hvis du vil tildele en rolle til gruppen, efter den er blevet oprettet, skal du gå til fanen **tildelte roller** for den netop oprettede gruppe og tildele rollen til gruppen.  

**Administrere medlemskab af en gruppe, der er tildelt til Azure AD-rolle**

For at undgå udvidelse af rettigheder kan det være, at administratorerne og globale administratorer som standard kun kan ændre medlemskabet af en gruppe, der er tildelt en rolle. De kan dog vælge at tildele en ejer af en sådan gruppe og uddelegere denne opgave.

Hvis du vil have mere at vide om at tildele Cloud-grupper til Azure AD-roller, skal du se [tildele en ad-roller til Cloud-gruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Du kan finde flere oplysninger om fejlfinding af roller, der er tildelt Cloud-grupper, under [fejlfinding af roller, der er tildelt Cloud-grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





