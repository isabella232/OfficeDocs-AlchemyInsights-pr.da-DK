---
title: Brugerbillede vises stadig i Microsoft Teams organisationsdiagram
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422214"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Brugerbillede vises stadig i Microsoft Teams organisationsdiagram

Hvis en eller flere personer i organisationen er blevet deaktiveret eller fjernet, og deres profilbillede stadig vises i organisationsdiagrammet, er det muligt, at **indstillingen ShowInAddressLists** er indstillet til Falsk: 

1. Gå til Microsoft 365 Administration > [aktive brugere,](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) og vælg brugeren med det billede, der stadig vises. 
1. Vælg fanen **Mail,** og sørg for, **at Vis i global adresseliste** er angivet til **Nej.**

Hvis indstillingen **ShowInAddressLists** **til Nej** ikke virker, skal du kontrollere følgende: 

- Brugeren kan vises på modtagerlisten i Exchange. Du kan få mere at vide [under Administrer adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Brugeren vises muligvis på adresselisten i Azure Active Directory. Du kan finde flere oplysninger [under Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 