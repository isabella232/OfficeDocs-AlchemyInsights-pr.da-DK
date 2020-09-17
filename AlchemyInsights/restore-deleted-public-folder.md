---
title: Gendanne en slettet offentlig mappe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774525"
---
# <a name="restore-a-deleted-public-folder"></a>Gendanne en slettet offentlig mappe

**Sådan gendanner du slettede elementer fra en offentlig mappe**:

- Se [du kan ikke gendanne slettede elementer fra en offentlig mappe, der ikke er mail i Outlook 2016](https://aka.ms/pfrec).
 
**Sådan gendannes en slettet offentlig mappe (af en hvilken som helst type)**: 

- Du kan bruge følgende EXO PowerShell-kommando:

    Stave

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Eksempel: følgende kommando gendanner Subfolder1 og placerer den under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Se [gendanne en slettet offentlig mappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for at få flere oplysninger.
