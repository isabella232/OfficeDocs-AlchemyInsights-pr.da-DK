---
title: UPN-synkronisering er deaktiveret
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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782145"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering er deaktiveret

Hvis du er begyndt at synkronisere med Azure AD før d. 30. marts 2016, skal du køre følgende Azure AD PowerShell-cmdlet for kun at aktivere UPN-blød match for din organisation:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-blød match er automatisk aktiveret for organisationer, der begyndte at synkronisere til Azure AD den eller efter d. 30. marts 2016.
  
Hvis du vil have mere at vide om at aktivere blød match på UPN og andre synkroniseringsfunktioner, skal du se [Azure AD Connect-synkroniseringstjenestefunktioner.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

