---
title: Flere brugere kan ikke se tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729865"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Flere brugere kan ikke se tilføjelsesprogrammer i Outlook

Hvis du tester Outlook-tilføjelsesprogrammer, og der ikke vises nogen, som det første trin til fejlfinding, skal du bruge **Get-OrganizationConfig PowerShell-** cmdlet'en til at forespørge _AppsForOfficeEnabled_ -parameteren. Hvis forespørgslen returnerer værdien **falsk**, skal du angive parameteren til **sand** ved hjælp af cmdlet'en **Set-OrganizationConfig** , så tilføjelsesprogrammer vises som forventet.

Vi anbefaler ikke, at parameteren _AppsForOfficeEnabled_ er angivet til **falsk**. En værdi på **falsk** tilsidesætter alle ovennævnte administrator-og brugerrolle indstillinger og forhindrer, at alle nye apps aktiveres af en bruger i organisationen.

Hvis du vil have mere at vide, skal du se [angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).