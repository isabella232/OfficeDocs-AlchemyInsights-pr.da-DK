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
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921702"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktiveret

Kør følgende Azure AD PowerShell cmdlet for at aktivere UPN bløde passer til din organisation kun, hvis du har startet synkroniseres til Azure AD inden 30 marts 2016:
  
 **Sæt MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn-Aktiver $True**
  
UPN bløde match er automatisk slået til organisationer, der synkroniseres til Azure AD på eller efter den 30. marts 2016 er startet.
  
For at få mere for at vide om aktivering af bløde match på UPN og andre funktioner, synkronisering, se [Azure AD Connect synkronisering service-funktioner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

