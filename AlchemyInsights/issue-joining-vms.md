---
title: Problem med at deltage i VM'er
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884980"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="f369d-102">Problem med at deltage i VM'er</span><span class="sxs-lookup"><span data-stu-id="f369d-102">Issue joining VMs</span></span>

<span data-ttu-id="f369d-103">Hvis du vil løse problemer, der opstår, når du forsøger at deltage i VM'er, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="f369d-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="f369d-104">Prøv at logge på ved hjælp af **UPN** -formatet (f. eks. ' joeuser@contoso.com ') i stedet for **sAMAccountName** -formatet (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="f369d-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="f369d-105">Kontrollér, at du har aktiveret synkronisering af adgangskoder i overensstemmelse med de trin, der er angivet i *introduktions* vejledning.</span><span class="sxs-lookup"><span data-stu-id="f369d-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="f369d-106">Kontrollér, at den pågældende brugerkonto ikke er en ekstern konto i Azure AD-lejeren.</span><span class="sxs-lookup"><span data-stu-id="f369d-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="f369d-107">Eksterne brugere kan ikke logge på det administrerede domæne, da Azure AD-domæne tjenester ikke har legitimationsoplysninger for sådanne brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="f369d-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="f369d-108">Hvis den pågældende brugerkonto er en skybaseret brugerkonto, skal du sørge for, at brugerne har ændret deres adgangskode, efter du har aktiveret Azure AD-domæne tjenester.</span><span class="sxs-lookup"><span data-stu-id="f369d-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="f369d-109">Dette trin medfører, at legitimationsoplysningerne for legitimationsoplysninger, der kræves for Azure AD-domæne tjenester oprettes.</span><span class="sxs-lookup"><span data-stu-id="f369d-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="f369d-110">Hvis de berørte brugerkonti synkroniseres fra en lokal adresseliste, skal du kontrollere, at den anbefalede version af Azure AD Connect er konfigureret til at udføre en fuld synkronisering.</span><span class="sxs-lookup"><span data-stu-id="f369d-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="f369d-111">Hvis problemet fortsætter, efter du har bekræftet trin 4, skal du udføre følgende kommandoer fra din synkroniserings maskine:</span><span class="sxs-lookup"><span data-stu-id="f369d-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="f369d-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="f369d-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>