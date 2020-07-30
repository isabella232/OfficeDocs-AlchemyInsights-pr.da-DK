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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522765"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte mail til arkivpostkassen

Hvis du vil have os til at køre automatiske kontroller for de indstillinger, der er nævnt nedenfor, skal du vælge tilbage-knappen < - øverst på denne side, og derefter indtaste e-mail-adressen på den bruger, der har problemer med at flytte e-mail til deres arkiv postkasse.

1. Bekræft, at **en arkivpostkasse** er aktiveret. Hvis ikke, skal du følge trinnene [i denne artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) for at aktivere arkivpostkassen.

2. Hvis du vil arkivere meddelelser automatisk i arkivpostkassen, skal en opbevaringskode **med handlingen Flyt** til arkiv indstilles til at **blive anvendt automatisk på hele postkassekoden (standardkode)**. Brug trinnene her for at oprette tagget: [Arkivér standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Føj derefter **arkivkoden til** din opbevaringspolitik. I Exchange Administration skal du vælge **Opbevaringspolitikker** > føje **tagget Flyt til arkiv** til politikken, > **gem**.

4. Tildel [nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse. Den samme politik anvendes på både primær- **og** **arkivkassen** Arkiv.

Det kan være nødvendigt at tvinge MFA (Managed Folder Assistant) til at køre og anvende de nye indstillinger på brugerens postkasse. Kør følgende kommando, mens du [har oprettet forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte assistenten For administreret mappe for en bestemt postkasse:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Du kan finde flere oplysninger om opsætning af en arkivpolitik [under Konfigurere en arkiv- og sletningspolitik for postkasser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  