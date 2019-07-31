---
title: Problemer, der logger på Office apps
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938175"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tom-logon-skærmen i Office-programmer

Du kan løse dette problem, kan du prøve følgende:
- Installere de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Nulstille indstillingerne i Internet Explorer: gå til **Tools** > **Internet-indstillinger** > **Avanceret** > **Reset Internet Explorer Settings** (Bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.
- Deaktiver Windows Defender-programmet Guard (WDAG) eller et tilsvarende firewall eller anti-virus program:
    1. Gå til **programmer**i Kontrolpanel, og vælg derefter **Slå Windows-funktioner til eller fra**.
    2. Hvis Windows Defender-programmet Guard er aktiveret, kan du prøve at deaktivere den.<br/>
    **Bemærk:** Du skal muligvis genstarte computeren.
- Sørg for, at Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokeres af et program eller en firewall antivirus-/ sikkerhedssoftware program.
- [Fjern Office legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.<br/>
    **Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Yderligere oplysninger finder du under [forbindelsen problemer i logon efter opdatering til Office 2016 build 16.0.7967 på Windows-10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).