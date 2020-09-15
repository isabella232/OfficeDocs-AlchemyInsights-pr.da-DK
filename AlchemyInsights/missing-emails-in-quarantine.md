---
title: Manglende mails i karantæne
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673708"
---
# <a name="missing-emails-in-quarantine"></a>Manglende mails i karantæne

Administratorer kan [få vist, udgive eller slette disse meddelelser.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Hvis du vil åbne sikkerheds & overholdelses Center, skal du gå til [https://protection.office.com](https://protection.office.com/) . Gå til for at åbne siden karantæne direkte [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan søge efterfølgende værdier:  

- **Meddelelses-id**: meddelelsens globalt entydige id. Hvis du vælger en meddelelse på listen, vises  **meddelelses-ID-**  værdien i pop op-ruden med  **detaljer**  , der vises. Administratorer kan bruge [meddelelsessporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til at finde meddelelser og deres tilsvarende meddelelses-id-værdier.
- **Afsender mailadresse**: en enkelt afsenders mailadresse.
- **Modtager mailadresse**: en enkelt modtagers mailadresse.
- **Emne**: Brug hele meddelelsens emne. Søgningen skelner ikke mellem store og små bogstaver.

Når du har angivet søgekriterierne, skal du klikke på Opdater ![ knap ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** for at filtrere resultaterne.  

De cmdletter, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:
- [Slet-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun gælder for meddelelser, ikke malware-filer fra DTT til SharePoint Online, OneDrive for Business eller teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)