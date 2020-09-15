---
title: Opret forbindelse til MSCommerce-modulet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713232"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="102cd-102">Opret forbindelse til MSCommerce-modulet</span><span class="sxs-lookup"><span data-stu-id="102cd-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="102cd-103">Du skal have forbindelse til modulet MSCommerce, før du kan få vist eller angive AllowSelfServicePurchase-politikken.</span><span class="sxs-lookup"><span data-stu-id="102cd-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="102cd-104">Hvis du vil oprette forbindelse til modulet MSCommerce, skal du i PowerShell-prompten (PS C: \) skal du skrive følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="102cd-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="102cd-105">Der åbnes en dialogboks til logon.</span><span class="sxs-lookup"><span data-stu-id="102cd-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="102cd-106">Indtast dit Brugernavn og din adgangskode for at logge på.</span><span class="sxs-lookup"><span data-stu-id="102cd-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="102cd-107">**Bemærk:** &nbsp; &nbsp; Den konto, der bruges til at logge på, skal være en virksomheds-eller fakturerings administrator.</span><span class="sxs-lookup"><span data-stu-id="102cd-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
