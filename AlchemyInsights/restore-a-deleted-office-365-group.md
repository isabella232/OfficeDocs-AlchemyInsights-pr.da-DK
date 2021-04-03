---
title: Gendan en slettet Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505680"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Gendan en slettet Microsoft 365-gruppe

Du kan gendanne en slettet Microsoft 365-gruppe eller Microsoft Teams inden for 30 dage efter sletningen.

1. Hvis du vil logge på Microsoft 365 Administration og oprette en liste over slettede grupper og teams, skal du gå til [Microsoft 365 Administration.](https://aka.ms/RestoreDeletedGroup)

    **Bemærk!** Log på med den konto, der er tildelt til enten lejeradministratoren eller gruppeadministratorrollen.

1. Vælg den slettede Microsoft 365-gruppe/Teams, der skal gendannes, og klik på **gendan gruppe.**

    Hvis gruppen ikke kan gendannes på grund af en SMTP-adresse, der er i konflikt med hinanden, skal du bruge følgende kommando til at finde det objekt, der forårsager konflikter, og fjerne SMTP-adressen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Bemærk!** I nogle tilfælde kan det tage helt op til 24 timer, før gruppen og alle dens data er gendannet.

    Du kan finde flere oplysninger eller få mere at vide om, hvordan du gendanner grupper ved hjælp af PowerShell, under [Gendan en slettet Microsoft 365-gruppe.](https://go.microsoft.com/fwlink/?linkid=867802)