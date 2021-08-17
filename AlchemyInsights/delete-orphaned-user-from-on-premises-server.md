---
title: Slet uafhængige brugere fra en server i det lokale miljø
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
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102239"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Slet uafhængige brugere fra en server i det lokale miljø

Hvis du vil fjerne en uafhængig bruger, skal du følge disse trin:

1. Gennemtving katalogsynkronisering ved at [følge vejledningen i Hvad er hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Se Hvad er hybrididentitet med Azure Active Directory? for [at bekræfte katalogsynkronisering.](https://technet.microsoft.com/library/jj151797.aspx)

3. Hvis synkronisering fungerer korrekt, men Active Directory-objektsletningen ikke overføres til Azure AD, skal du manuelt fjerne det uafhængige objekt ved hjælp af en af følgende Azure Active Directory-modul til Windows PowerShell-cmdlet'er:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Hvis du f.eks. vil fjerne uafhængige bruger-john.smith@contoso.com, der oprindeligt blev oprettet ved hjælp af katalogsynkronisering, skal du køre cmdlet'en:

    Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com