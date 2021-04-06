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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597437"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="0b49e-102">Gendan en slettet Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="0b49e-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="0b49e-103">Du kan gendanne en slettet Microsoft 365-gruppe eller Microsoft Teams inden for 30 dage efter sletningen.</span><span class="sxs-lookup"><span data-stu-id="0b49e-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="0b49e-104">Gå til [Microsoft 365 Administration for at logge](https://aka.ms/RestoreDeletedGroup) på og få vist de slettede grupper og teams.</span><span class="sxs-lookup"><span data-stu-id="0b49e-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="0b49e-105">**Bemærk!** Log på med den konto, der er tildelt administratorlejeren eller gruppeadministratorrollen.</span><span class="sxs-lookup"><span data-stu-id="0b49e-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="0b49e-106">Vælg den slettede Microsoft 365-gruppe/Teams, der skal gendannes, og klik på **Gendan gruppe.**</span><span class="sxs-lookup"><span data-stu-id="0b49e-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="0b49e-107">Hvis gruppen ikke kan gendannes på grund af en SMTP-adresse, der skaber konflikt, skal du bruge følgende kommando til at finde det objekt, der forårsager konflikter, og fjerne SMTP-adressen:</span><span class="sxs-lookup"><span data-stu-id="0b49e-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="0b49e-108">**Bemærk!** I nogle tilfælde kan det tage helt op til 24 timer, før gruppen og alle dens data er gendannet.</span><span class="sxs-lookup"><span data-stu-id="0b49e-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="0b49e-109">Du kan finde flere oplysninger eller få mere at vide om, hvordan du gendanner grupper ved hjælp af PowerShell, under [Gendan en slettet Microsoft 365-gruppe.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="0b49e-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>