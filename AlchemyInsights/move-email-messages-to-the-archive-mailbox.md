---
title: Flytte mails til postkassen Arkiv
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713640"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte mail til arkivpostkassen

1. Bekræft, at en **arkivpostkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere arkivpostkassen.

2. Hvis du vil arkivere meddelelser automatisk til arkivpostkassen, skal et opbevaringsmærke med handlingen **Flyt til arkiv** angives til **automatisk at blive anvendt på hele postkassekoden (standard).** Følg trinnene her for at oprette mærket: [Arkivstandardkode](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Derefter skal du føje **arkivtagget** til din opbevaringspolitik. I Exchange Administration skal du vælge **Opbevaringspolitikker >** føje **tagget Flyt til arkiv** til politikken > **Gem**.

4. [Tildel nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse. Den samme politik anvendes på både postkassen **Primær** og **Arkiv.**

Det kan være nødvendigt at tvinge MFA (Managed Folder Assistant) til at køre og anvende de nye indstillinger på brugerens postkasse. Kør følgende kommando, mens [du har forbindelse til EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte Assistent til administrerede mapper for en bestemt postkasse:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Du kan finde flere oplysninger om opsætning af en arkivpolitik [under Konfigurere en arkiv- og sletningspolitik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  