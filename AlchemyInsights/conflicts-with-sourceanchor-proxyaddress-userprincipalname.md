---
title: Konflikter med SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 2d58078fcabb416c418b67a2f2ce2eba679a18c6ecf3846c534bde74188d7827
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033056"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a>Konflikter med SourceAnchor, ProxyAddress, UserPrincipalName

Hvis du modtager fejl under en synkronisering, f.eks. "Et synkroniseret objekt med samme ProxyAddress eller UserPrincipalName findes i din mappe", skal du se [Diagnosticere](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)og løse duplikerede synkroniseringsfejl med attributter.

Du bør også overveje at aktivere duplikerede attribut-fleksibilitet. Du kan få mere at vide under [Identitetssynkronisering og duplikerede attributters fleksibilitet.](https://aka.ms/duplicateattributeresiliency)