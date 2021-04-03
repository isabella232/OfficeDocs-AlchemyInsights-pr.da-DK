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
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="a3ad8-102">Gendan en slettet Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="a3ad8-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="a3ad8-103">Du kan gendanne en slettet Microsoft 365-gruppe eller Microsoft Teams inden for 30 dage efter sletningen.</span><span class="sxs-lookup"><span data-stu-id="a3ad8-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="a3ad8-104">Hvis du vil logge på Microsoft 365 Administration og oprette en liste over slettede grupper og teams, skal du gå til [Microsoft 365 Administration.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="a3ad8-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="a3ad8-105">**Bemærk!** Log på med den konto, der er tildelt til enten lejeradministratoren eller gruppeadministratorrollen.</span><span class="sxs-lookup"><span data-stu-id="a3ad8-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="a3ad8-106">Vælg den slettede Microsoft 365-gruppe/Teams, der skal gendannes, og klik på **gendan gruppe.**</span><span class="sxs-lookup"><span data-stu-id="a3ad8-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="a3ad8-107">Hvis gruppen ikke kan gendannes på grund af en SMTP-adresse, der er i konflikt med hinanden, skal du bruge følgende kommando til at finde det objekt, der forårsager konflikter, og fjerne SMTP-adressen:</span><span class="sxs-lookup"><span data-stu-id="a3ad8-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="a3ad8-108">**Bemærk!** I nogle tilfælde kan det tage helt op til 24 timer, før gruppen og alle dens data er gendannet.</span><span class="sxs-lookup"><span data-stu-id="a3ad8-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="a3ad8-109">Du kan finde flere oplysninger eller få mere at vide om, hvordan du gendanner grupper ved hjælp af PowerShell, under [Gendan en slettet Microsoft 365-gruppe.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="a3ad8-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>