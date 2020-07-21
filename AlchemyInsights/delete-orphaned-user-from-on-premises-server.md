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
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="d52ac-102">Slet forældreløse bruger fra den lokale server</span><span class="sxs-lookup"><span data-stu-id="d52ac-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="d52ac-103">FÃ ̧lg disse trin for at fjerne en bruger, der ikke er forældre eller en bruger, der er forældreløs:</span><span class="sxs-lookup"><span data-stu-id="d52ac-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="d52ac-104">Gennemtving katalogsynkronisering ved at følge instruktionerne i [Hvad er hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="d52ac-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="d52ac-105">Hvis du vil bekræfte katalogsynkronisering, skal du se [Hvad er hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="d52ac-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="d52ac-106">Hvis synkronisering fungerer korrekt, men sletningen af Active Directory-objektet ikke overføres til Azure AD, skal du manuelt fjerne det forældreløse objekt ved hjælp af et af følgende Azure Active Directory-moduler til Windows PowerShell-cmdletter:</span><span class="sxs-lookup"><span data-stu-id="d52ac-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="d52ac-107">Fjern-MsolContact</span><span class="sxs-lookup"><span data-stu-id="d52ac-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="d52ac-108">Fjern-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="d52ac-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="d52ac-109">Fjern-MsolUser</span><span class="sxs-lookup"><span data-stu-id="d52ac-109">Remove-MsolUser</span></span>

    <span data-ttu-id="d52ac-110">Hvis du for eksempel vil fjerne forældreløse bruger-id-john.smith@contoso.com, der oprindeligt blev oprettet ved hjælp af katalogsynkronisering, skal du køre cmdlet'en:</span><span class="sxs-lookup"><span data-stu-id="d52ac-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="d52ac-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="d52ac-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>