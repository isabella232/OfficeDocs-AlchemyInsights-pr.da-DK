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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038106"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering er deaktiveret

Hvis du er begyndt at synkronisere med Azure AD før d. 30. marts 2016, skal du køre følgende Azure AD PowerShell-cmdlet for kun at aktivere UPN-blød match for din organisation:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-blød match er automatisk aktiveret for organisationer, der begyndte at synkronisere til Azure AD den eller efter d. 30. marts 2016.
  
Hvis du vil have mere at vide om at aktivere blød match på UPN og andre synkroniseringsfunktioner, skal du se [Azure AD Forbind-synkroniseringstjenestefunktioner.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

