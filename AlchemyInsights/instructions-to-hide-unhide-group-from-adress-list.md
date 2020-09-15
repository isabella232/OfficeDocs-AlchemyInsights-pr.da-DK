---
title: Vejledning til at skjule/vise en gruppe fra adresselisten
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663003"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="3c050-102">Skjul Microsoft 365-gruppe fra adresseliste (GAL)</span><span class="sxs-lookup"><span data-stu-id="3c050-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="3c050-103">Hvis du vil skjule en Microsoft 365-gruppe fra en adresseliste (GAL) af Exchange-klienter (f. eks Outlook eller OWA), skal du bruge følgende kommando i EXO shell:</span><span class="sxs-lookup"><span data-stu-id="3c050-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="3c050-104">Hvis du vil skjule Microsoft 365-gruppen fra at blive synlig for Exchange-klienter, skal du bruge følgende kommando i EXO shell:</span><span class="sxs-lookup"><span data-stu-id="3c050-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

