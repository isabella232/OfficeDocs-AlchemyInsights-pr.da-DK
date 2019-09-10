---
title: Flytte mails til arkivpostkassen
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
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822156"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte mails til arkivpostkassen

1. Bekræft, at en **arkivpostkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere arkivpostkassen.

2. Hvis du vil arkivere meddelelser automatisk i arkivpostkassen, skal en opbevaringskode med handlingen **Flyt til arkiv** være indstillet til **automatisk anvendt på hele postkasse koden (standard)**. Brug trinnene her til at oprette tagget: [Arkiv standardtag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Derefter skal du føje **arkiverings** tagget til din opbevaringspolitik. I Exchange administration skal du vælge **opbevaringspolitikker** > føje **Flyt til arkiv-tagget** til politikken > **Gem**.

4. [Tildel nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse. Den samme politik vil blive anvendt på både den **primære** postkasse og **Arkiv** postkassen.

Det kan være nødvendigt at tvinge den administrerede mappe assistent (MFA) til at køre og anvende de nye indstillinger på brugerens postkasse. Kør følgende kommando, mens [du har forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte den administrerede mappe assistent for en bestemt postkasse:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Du finder flere oplysninger om, hvordan du konfigurerer en arkiveringspolitik, i [konfigurere en arkiverings-og sletningspolitik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  