---
title: Flyt mails til arkiv postkassen
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799774"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte mails til arkiv postkassen

Hvis du vil have os til at køre automatiske tjek af de indstillinger, der er nævnt nedenfor, skal du vælge knappen tilbage <-øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med at flytte mail til deres Arkiv postkasse.

1. Bekræft, at en **Arkiv postkasse** er blevet aktiveret. Hvis ikke, skal du følge trinnene i [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) for at aktivere Arkiv postkassen.

2. Hvis du vil arkivere meddelelser automatisk til arkiv postkassen, skal et opbevarings mærke med handlingen **Flyt til arkiv** være indstillet til **automatisk at blive anvendt på hele postkassen (standard)-mærket**. Følg trinnene her for at oprette mærket: [arkiverings standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Derefter skal du tilføje **Arkiv** mærket til opbevaringspolitikken. I Exchange Admin Center skal du vælge **opbevaringspolitikker** > føje **Flyt til arkiv-mærket** til politik > **gemme**.

4. Nu kan du [tildele opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den pågældende brugers postkasse. Den samme politik anvendes på både den **primære** og den **arkiverede** postkasse.

Det kan være nødvendigt at gennemtvinge, at MFA (Managed folder Assistant) kører og anvende de nye indstillinger i brugerens postkasse. Kør følgende kommando, mens [du har forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte en administreret mappe assistent til en bestemt postkasse:
  
Start-ManagedFolderAssistant-id <name of the mailbox>

Hvis du vil have mere at vide om konfiguration af en Arkiv politik, skal du se [konfigurere en arkiv-og sletnings politik for postkasser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  