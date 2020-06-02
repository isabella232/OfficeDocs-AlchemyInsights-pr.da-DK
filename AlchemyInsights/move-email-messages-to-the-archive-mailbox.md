---
title: Flytte mails til arkivpostkassen
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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511034"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte mail til arkivpostkassen

1. Bekræft, at en **arkivpostkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) til at aktivere arkivpostkassen.

2. Hvis du vil arkivere meddelelser automatisk i arkivkassen, skal der angives en opbevaringskode med handlingen **Flyt til arkiv** **automatisk, så den automatisk anvendes på hele postkassekoden (standard).** Følg trinnene her for at oprette koden: [Arkivstandardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Derefter skal du føje **arkivtagget** til din opbevaringspolitik. I Exchange Administration skal du vælge **Opbevaringspolitikker** > føje **tagget Flyt til arkiv** til politikken > **Gem**.

4. [Tildel nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse. Den samme politik anvendes på både postkassen **Primær** og **Arkiv.**

Det kan være nødvendigt at tvinge MFA (Managed Folder Assistant) til at køre og anvende de nye indstillinger på brugerens postkasse. Kør følgende kommando, mens [du har forbindelse til EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte assistenten for administrerede mapper for en bestemt postkasse:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Du kan finde flere oplysninger om opsætning af en arkivpolitik under [Konfigurere en arkiv- og sletningspolitik for postkasser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  