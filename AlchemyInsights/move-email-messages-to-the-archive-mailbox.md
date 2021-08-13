---
title: Flyt mails til arkivpostkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974951"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flyt mail til arkivpostkassen

Hvis du vil have os til at køre automatiserede kontroller af de indstillinger, der er nævnt nedenfor, skal du vælge knappen Tilbage < – øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med at flytte mails til arkivpostkassen.

1. Bekræft, at **en Arkivpostkasse** er blevet aktiveret. Hvis ikke, skal du følge trinnene i [denne artikel for](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) at aktivere arkivpostkassen.

2. For at arkivere meddelelser automatisk til arkivpostkassen, skal et opbevaringsmærke med handlingen Flyt til arkiv være indstillet til at anvendes automatisk på **hele postkassen (standard) mærke**.  Brug trinnene her for at oprette mærket: [Arkiveringsstandardmærke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Derefter skal du føje **arkivmærket** til din opbevaringspolitik. I administration Exchange skal du vælge **Opbevaringspolitikker,** >  du føje mærket Flyt til arkiv til politikken > **Gem.**

4. Tildel [opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse. Den samme politik anvendes på både **primær- og** **arkivpostkassen.**

Det kan være nødvendigt at gennemtvinge, at den administrerede mappeassistent (MFA) kører og anvender de nye indstillinger på brugerens postkasse. Kør følgende kommando, mens du [har forbindelse til EXO PowerShell for](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) at starte en administreret mappeassistent for en bestemt postkasse:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Du kan finde flere oplysninger om konfiguration af en arkiveringspolitik [under Konfigurer en arkiverings- og sletningspolitik for postkasser.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  