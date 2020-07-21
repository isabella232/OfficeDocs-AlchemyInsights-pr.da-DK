---
title: Slet forældreløse bruger fra den lokale server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197942"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Slet forældreløse bruger fra den lokale server

FÃ ̧lg disse trin for at fjerne en bruger, der ikke er forældre eller en bruger, der er forældreløs:

1. Gennemtving katalogsynkronisering ved at følge instruktionerne i [Hvad er hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Hvis du vil bekræfte katalogsynkronisering, skal du se [Hvad er hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx)

3. Hvis synkronisering fungerer korrekt, men sletningen af Active Directory-objektet ikke overføres til Azure AD, skal du manuelt fjerne det forældreløse objekt ved hjælp af et af følgende Azure Active Directory-moduler til Windows PowerShell-cmdletter:

    Fjern-MsolContact  
    Fjern-MsolGroup  
    Fjern-MsolUser

    Hvis du for eksempel vil fjerne forældreløse bruger-id-john.smith@contoso.com, der oprindeligt blev oprettet ved hjælp af katalogsynkronisering, skal du køre cmdlet'en:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com