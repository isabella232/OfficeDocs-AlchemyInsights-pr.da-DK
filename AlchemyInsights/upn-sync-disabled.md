---
title: UPN-synkronisering deaktiveret
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423537"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktiveret

Kør følgende Azure AD PowerShell cmdlet for at aktivere UPN bløde passer til din organisation kun, hvis du har startet synkroniseres til Azure AD inden 30 marts 2016:
  
 **Sæt MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn-Aktiver $True**
  
UPN bløde match er automatisk slået til organisationer, der synkroniseres til Azure AD på eller efter den 30. marts 2016 er startet.
  
For at få mere for at vide om aktivering af bløde match på UPN og andre funktioner, synkronisering, se [Azure AD Connect synkronisering service-funktioner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

