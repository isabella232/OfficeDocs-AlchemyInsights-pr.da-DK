---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695281"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tomt logonskærmbillede i Microsoft 365-apps

Prøv følgende for at løse dette problem:
- Installer de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Nulstil indstillinger for Internet Explorer: gå til **funktioner**  >  **Internetindstillinger**  >  **Avanceret**  >  **Nulstil indstillinger for Internet Explorer** (Bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.
- Deaktiver Windows Defender Application Guard (WDAG) eller lignende firewall-eller antivirusprogram:
    1. I kontrol panel skal du gå til **programmer**og derefter vælge **slå Windows-funktioner til eller fra**.
    2. Hvis Windows Defender Application Guard er aktiveret, kan du prøve at deaktivere det.<br/>
    **Bemærk:** Du skal muligvis genstarte computeren.
- Kontrollér, at [WAM-plug-in'en](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) for Microsoft. Aad. BrokerPlugin Aad ikke blokeres af programmer eller firewall/antivirusprogrammer.
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.<br/>
    **Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0. (F. eks.: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil have mere at vide, skal du se [forbindelsesproblemer i logon efter opdatering til Office 2016 Build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).