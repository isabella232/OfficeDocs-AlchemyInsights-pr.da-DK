---
title: UPN-synkronisering deaktiveret
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749508"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktiveret

Hvis du begyndte at synkronisere til Azure AD før 30. marts 2016, skal du køre følgende Azure AD PowerShell-cmdlet for at aktivere UPN – kun for din organisation:
  
 **Set-MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn – aktivere $True**
  
Blødt UPN-match er automatisk slået til for organisationer, der begyndte at synkronisere til Azure AD på eller efter 30. marts 2016.
  
Hvis du vil have mere at vide om at aktivere blødt match på UPN og andre synkroniseringsfunktioner, skal du se [Azure ad Connect-tjenesten Sync-funktioner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

