---
title: Brugerbillede vises ikke i Microsoft Teams organisationsdiagram
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792690"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Brugerbillede vises ikke i Microsoft Teams organisationsdiagram

Hvis en eller flere personer i organisationen mangler deres profilbillede i organisationsdiagrammet, er det muligt, at **indstillingen ShowInAddressLists** er angivet til **Falsk:**

1. Gå til Microsoft 365 Administration > [**Aktive brugere**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), og vælg brugeren med det manglende billede. 
1. Vælg fanen **Mail,** og sørg for, at **Vis i global adresseliste** er indstillet til **Ja**. 

Hvis indstillingen **ShowInAddressLists** **til Ja** ikke virker, skal du kontrollere følgende:

- Brugeren kan være skjult på modtagerlisten i Exchange. Du kan få mere at [vide under Administrer adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Brugeren kan være skjult fra adresselisten i Azure Active Directory. Du kan finde flere oplysninger [under Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
