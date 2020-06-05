---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579895"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom logonskærm i Microsoft 365-apps

Du kan løse dette problem ved at prøve følgende:
- Installer de nyeste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Nulstil indstillinger for Internet Explorer: Gå til **Funktioner**  >  **Internetindstillinger**  >  **Avancerede**  >  **Nulstil indstillinger i Internet Explorer** (bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.
- Deaktiver Windows Defender Application Guard (WDAG) eller et lignende firewall- eller antivirusprogram:
    1. Gå til Programmer **i**Kontrolpanel , og vælg derefter **Slå Windows-funktioner**til eller fra .
    2. Hvis Windows Defender Application Guard er aktiveret, kan du prøve at deaktivere den.<br/>
    **Bemærk:** Det kan være nødvendigt at genstarte computeren.
- Kontroller, at microsoft.AAD.BrokerPlugin [AAD WAM-plug-in'en](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokeres af programmer eller firewall-/antivirusprogram.
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.<br/>
    **Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0. (Eks.: \Software\Microsoft\Office\16.0\Common\Identity\)

Du kan finde flere oplysninger [under Forbindelsesproblemer ved logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).