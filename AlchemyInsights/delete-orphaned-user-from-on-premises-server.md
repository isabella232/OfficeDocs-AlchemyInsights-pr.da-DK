---
title: Slet mistede brugere fra lokal server
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680129"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Slet mistede brugere fra lokal server

Hvis du vil fjerne en tabt bruger, skal du følge disse trin:

1. Gennemtving Katalogsynkronisering ved at følge vejledningen i [Hvad er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Hvis du vil bekræfte Katalogsynkronisering, skal du se [Hvad er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Hvis Synkroniser fungerer korrekt, men Active Directory-objekt sletningen ikke overføres til Azure AD, skal du fjerne det mistede objekt manuelt ved hjælp af et af følgende Azure Active Directory-modul til Windows PowerShell-cmdletter:

    Fjern-MsolContact  
    Fjern-MsolGroup  
    Fjern-MsolUser

    Hvis du f. eks fjerner et barneret bruger-ID john.smith@contoso.com, der oprindeligt blev oprettet ved hjælp af katalogsynkronisering, skal du køre cmdlet'en:

    Fjern-MsolUser – UserPrincipalName John.Smith@Contoso.com