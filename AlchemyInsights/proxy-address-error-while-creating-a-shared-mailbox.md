---
title: Proxyadressefejl under oprettelse af en delt postkasse
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568284"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="8e594-102">Proxyadressefejl under oprettelse af en postkasse eller et andet mailaktiveret objekt</span><span class="sxs-lookup"><span data-stu-id="8e594-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="8e594-103">Hvis du forsøgte at oprette et mailaktiveret objekt (postkasse, delt postkasse osv.) og modtog fejlen "Proxyadressen "SMTP:alias@domain.com" er allerede i brug...", så er den mailadresse, du har valgt, allerede taget af et andet mailaktiveret objekt i organisationen.</span><span class="sxs-lookup"><span data-stu-id="8e594-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="8e594-104">Du skal finde den bruger, gruppe, delte postkasse eller offentlige mappe, der har denne mailadresse, og slette den eller ændre dens mailadresse.</span><span class="sxs-lookup"><span data-stu-id="8e594-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="8e594-105">Derefter kan du oprette et nyt mailaktiveret objekt med den frigjorte mailadresse.</span><span class="sxs-lookup"><span data-stu-id="8e594-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="8e594-106">Brug Søg på startsiden til at finde den.</span><span class="sxs-lookup"><span data-stu-id="8e594-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="8e594-107">Du kan også bruge følgende Exchange Online PowerShell-kommando til at søge efter den:</span><span class="sxs-lookup"><span data-stu-id="8e594-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="8e594-108">Hvis du ikke vil slette den eksisterende mailadresse, skal du vælge en ny mailadresse til det nye objekt, du opretter.</span><span class="sxs-lookup"><span data-stu-id="8e594-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  