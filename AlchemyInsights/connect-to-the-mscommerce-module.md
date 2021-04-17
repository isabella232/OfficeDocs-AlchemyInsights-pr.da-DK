---
title: Opret forbindelse til MSCommerce-modulet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: e77c6a329ac99a4cea4f143dcb3c661b6a518e35
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817022"
---
# <a name="connect-to-the-mscommerce-module"></a>Opret forbindelse til MSCommerce-modulet

Du skal have forbindelse til MSCommerce-modulet, før du kan få vist eller angive politikken AllowSelfServicePurchase.  

Hvis du vil oprette forbindelse til modulet MSCommerce, skal du skrive følgende kommando i PowerShell-prompten (PS \) C: :

`Connect-MSCommerce`

Dette åbner en dialogboks til logon. Angiv dit brugernavn og din adgangskode for at logge på.

**BEMÆRK!** &nbsp; &nbsp; Den konto, der bruges til at logge på, skal være en virksomhed eller faktureringsadministrator.
