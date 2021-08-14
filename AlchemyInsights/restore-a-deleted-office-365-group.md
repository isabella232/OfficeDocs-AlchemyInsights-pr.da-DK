---
title: Gendanne en slettet Microsoft 365 gruppe
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959020"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Gendanne en slettet Microsoft 365 gruppe

Du kan gendanne en slettet Microsoft 365 en gruppe eller Microsoft Teams inden for 30 dage efter sletningen.

1. Gå til [Microsoft 365 Administration](https://aka.ms/RestoreDeletedGroup) for at logge på en liste over dine slettede grupper og teams.

    **Bemærk!** Log på med den konto, der er tildelt administratorlejeren eller gruppeadministratorrollen.

1. Vælg den slettede Microsoft 365/gruppe/gruppe Teams skal gendannes, og klik på **Gendan gruppe**.

    Hvis gruppen ikke kan gendannes på grund af en SMTP-adresse, der skaber konflikt, skal du bruge følgende kommando til at finde det objekt, der forårsager konflikter, og fjerne SMTP-adressen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Bemærk!** I nogle tilfælde kan det tage helt op til 24 timer, før gruppen og alle dens data er gendannet.

    Du kan finde flere oplysninger eller få mere at vide om, hvordan du gendanner grupper ved hjælp af PowerShell, [under Gendan en slettet Microsoft 365 gruppe](https://go.microsoft.com/fwlink/?linkid=867802).