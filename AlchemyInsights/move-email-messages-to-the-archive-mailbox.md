---
title: Flytte e-mails til postkassen arkiv
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36548997"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte e-mails til postkassen arkiv

1. Bekræft, at en **arkivere postkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere postkassen arkiv.

2. For at arkivere meddelelser automatisk til arkiv-postkasse, skal være angivet en tilbageholdelse kode med handlingen, der **flytter til arkiv** der **anvendes automatisk til hele postkasse (standard) mærke**. Brug vejledningen her til at oprette mærket: [arkivet standard mærke](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Dernæst skal du tilføje koden **arkiv** til din opbevaringspolitik. Vælg **Opbevaringspolitikker** i Exchange admin center, > føje **flytter til arkiv mærke** til politik > **Gem**.

4. Nu [tildele opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til brugerens postkasse. Denne politik anvendes til både den **primære** og **arkiv** -postkasse.

Det kan være nødvendigt at tvinge den administrerede mappe assistenten (MFA) til at køre og anvende de nye indstillinger i brugerens postkasse. Kør følgende kommando under [tilsluttet EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) til at starte en administreret Mappeassistent for en bestemt postkasse:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Yderligere oplysninger om opsætning af en arkiveringspolitik, se [oprette et arkiv og sletning af en politik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  