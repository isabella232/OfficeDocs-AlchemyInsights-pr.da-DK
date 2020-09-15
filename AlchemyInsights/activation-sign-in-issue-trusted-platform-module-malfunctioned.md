---
title: Problem med aktivering/logon – Trusted Platform modul fungerer ikke
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
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697515"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Rettelse af Microsoft 365-apps "din computers Trusted Platform-modul fungerer ikke korrekt"-meddelelse

Du kan rette fejlen ved at følge disse trin:

1. Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti.   
2. Brug af Windows- **indstillings**  >  **konti**  >  **mail & konti**, Fjern eksisterende arbejds konti. 
3. Brug af Windows- **indstillings**  >  **konti**  >  **adgang til arbejde eller skole**, Afbryd forbindelsen til eksisterende konti. 
4. Nulstil aktiveringstilstand for Office. [Lær hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Prøv [genoprettelsesprocessen for brugeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at løse TPM-fejl (Trusted Platform Module).