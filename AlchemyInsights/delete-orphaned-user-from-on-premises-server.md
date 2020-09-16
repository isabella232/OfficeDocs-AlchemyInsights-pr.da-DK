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
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="208aa-102">Slet mistede brugere fra lokal server</span><span class="sxs-lookup"><span data-stu-id="208aa-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="208aa-103">Hvis du vil fjerne en tabt bruger, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="208aa-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="208aa-104">Gennemtving Katalogsynkronisering ved at følge vejledningen i [Hvad er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="208aa-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="208aa-105">Hvis du vil bekræfte Katalogsynkronisering, skal du se [Hvad er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="208aa-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="208aa-106">Hvis Synkroniser fungerer korrekt, men Active Directory-objekt sletningen ikke overføres til Azure AD, skal du fjerne det mistede objekt manuelt ved hjælp af et af følgende Azure Active Directory-modul til Windows PowerShell-cmdletter:</span><span class="sxs-lookup"><span data-stu-id="208aa-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="208aa-107">Fjern-MsolContact</span><span class="sxs-lookup"><span data-stu-id="208aa-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="208aa-108">Fjern-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="208aa-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="208aa-109">Fjern-MsolUser</span><span class="sxs-lookup"><span data-stu-id="208aa-109">Remove-MsolUser</span></span>

    <span data-ttu-id="208aa-110">Hvis du f. eks fjerner et barneret bruger-ID john.smith@contoso.com, der oprindeligt blev oprettet ved hjælp af katalogsynkronisering, skal du køre cmdlet'en:</span><span class="sxs-lookup"><span data-stu-id="208aa-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="208aa-111">Fjern-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="208aa-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>