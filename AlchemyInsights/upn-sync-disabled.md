---
title: UPN-synkronisering deaktiveret
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532325"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="ee516-102">UPN-synkronisering deaktiveret</span><span class="sxs-lookup"><span data-stu-id="ee516-102">UPN sync disabled</span></span>

<span data-ttu-id="ee516-103">Kør følgende Azure AD PowerShell cmdlet for at aktivere UPN bløde passer til din organisation kun, hvis du har startet synkroniseres til Azure AD inden 30 marts 2016:</span><span class="sxs-lookup"><span data-stu-id="ee516-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="ee516-104">**Sæt MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn-Aktiver $True**</span><span class="sxs-lookup"><span data-stu-id="ee516-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="ee516-105">UPN bløde match er automatisk slået til organisationer, der synkroniseres til Azure AD på eller efter den 30. marts 2016 er startet.</span><span class="sxs-lookup"><span data-stu-id="ee516-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="ee516-106">For at få mere for at vide om aktivering af bløde match på UPN og andre funktioner, synkronisering, se [Azure AD Connect synkronisering service-funktioner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="ee516-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

