---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833025"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom logonskærm i Microsoft 365-apps

Du kan løse dette problem ved at prøve følgende:
- Installér de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Nulstil indstillinger i Internet Explorer: Gå til Værktøjer Internetindstillinger Avanceret Nulstil  >    >    >  **indstillinger i Internet Explorer** (bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.
- Deaktiver Windows Defender Application Guard (WDAG) eller en lignende firewall eller et antivirusprogram:
    1. I Kontrolpanel skal du gå **til Programmer** og derefter vælge **Slå Windows-funktioner til eller fra**.
    2. Hvis Windows Defender Application Guard er aktiveret, kan du prøve at deaktivere den.<br/>
    **Bemærk!** Du skal muligvis genstarte computeren.
- Sørg for, at plug-in'en Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokeres af nogen applikation eller firewall/antivirusprogram.
- [Ryd Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.<br/>
    **Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0. (Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)

Du kan få mere at vide under Forbindelsesproblemer ved logon efter opdatering til [Office 2016 build 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)