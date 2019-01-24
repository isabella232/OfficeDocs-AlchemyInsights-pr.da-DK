---
title: Flytte e-mails til postkassen arkiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464159"
---
Problemer med arkivering af elementer til arkiv-postkasse. Kontroller, at du har udført følgende trin:
  
1. Bekræft, at en **arkivere postkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) til at aktivere postkassen arkiv. 
    
2. Vælg **Tilbageholdelse mærker** under **Administration af overholdelse**i administrationssiden Exchange, oprette en **tilbageholdelse mærke** med handlingen **flytter til arkiv** , der indeholder den ønskede **Tilbageholdelse alder**.
    
3. Vælg **Opbevaringspolitikker**i Exchange Admin Center, Opret en **Opbevaringspolitik** , og Tilføj **flytter til arkiv** tilbageholdelse af mærket til denne politik. 
    
4. [Tildele opbevaringspolitikken](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til brugerens postkasse. Denne politik anvendes til både den **primære** og **arkiv** -postkasse. 
    
Brugerens postkasse skulle nu være en arkiveringspolitik til at flytte varer til arkiv-postkasse. Det kan være nødvendigt at tvinge den administrerede mappe assistenten (MFA) til at køre og anvende de nye indstillinger i brugerens postkasse. Kør følgende kommando under [tilsluttet EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) til at starte en administreret Mappeassistent for en bestemt postkasse: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Vil have yderligere oplysninger om opsætning af en arkiveringspolitik, finder du i [oprette et arkiv og sletning af en politik for postkasser](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

