---
title: Gendanne en slettet offentlig mappe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063622"
---
# <a name="restore-a-deleted-public-folder"></a>Gendanne en slettet offentlig mappe

**Sådan gendannes slettede elementer fra en offentlig mappe:**

- Se [Du kan ikke gendanne slettede elementer fra en offentlig mappe, der ikke er e-mail, i Outlook 2016](https://aka.ms/pfrec).
 
**Sådan gendannes en slettet offentlig mappe (af enhver type):** 

- Brug følgende EXO PowerShell-kommando:

    Syntaks:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Stisti, hvor mappen gendannes>

    Eksempel: Følgende kommando gendanner Undermappe1 og placerer den under \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq "Undermappe1"}; Set-PublicFolder $pf.identity -Sti \Parent1

Se [Gendanne en slettet offentlig mappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for at få flere oplysninger.
