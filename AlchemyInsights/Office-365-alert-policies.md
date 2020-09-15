---
title: 1385 – Office-365-Alert-Policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664020"
---
# <a name="alert-policies"></a>Påmindelses politikker

Microsoft 365 Security & overholdelses Center indeholder [standard påmindelses politikker](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) , der udløser beskeder for organisationer med et Office 365 Enterprise-eller Office 365 amerikanske--, E3/G3-eller E5/G5-abonnement. Derfor modtager administratorerne en meddelelse om en advarsel via mail, der sendes af Office365Alerts@microsoft.com med en emnelinje, f. eks "en lav prioritet: *navnet på besked politikken*". Påmindelser sendes, når der udløses påmindelser for almindelige aktiviteter, f. eks når brugere:

- Opret indbakkeregler, der videresender mail.
- Tildel tilladelser til deres postkasse.
- Del eller slet et stort antal filer i SharePoint-fildeling.
- Opret eDiscovery-søgninger, og eksportér søgeresultater.

Sådan gennemser og reagerer en besked:

1. Gå til [Security & Overholdelsescenter](https://protection.office.com) , og log på.
2. Klik på **beskeder**  >  **Vis beskeder**.
3. Klik på en besked for at få vist en pop op-side med oplysninger om beskeden.

Du kan reagere på en besked, f. eks at [fjerne en mistænkelig indbakke regel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Du kan også lukke beskeden ved at klikke på **løs** på pop op-siden med advarslen.

Du kan finde flere oplysninger om, hvordan du konfigurerer og administrerer påmindelses politikker, i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Vigtigt**! besked om påmindelse via mail fra Microsoft vil aldrig bede dig om at gøre følgende:

- Angive en adgangskode
- Bekræft sikkerheds detaljerne for din konto
- Godkend dig selv igen

Hvis du modtager en mail som denne, blev den ikke sendt af Microsoft, og det anses for at være en phishing-bedrageri. Hvis det sker, skal du [rapportere det til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).