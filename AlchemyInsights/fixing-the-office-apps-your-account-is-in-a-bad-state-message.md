---
title: Fastsættelse af Office-apps Din konto er i en meddelelse om dårlig tilstand
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969341"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Rette op på Office-appsene "Din konto er i dårlig tilstand"-fejl

Du kan løse denne fejl ved at prøve følgende indstillinger på den berørte computer:

- Åbn en Office-app, vælg Log på **filer** > **konto** > **af alle konti**. Log på igen ved hjælp af en brugerkonto med en gyldig licens. Du kan finde detaljerede oplysninger under [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Credential Manager.<br>
  **Bemærk:** Registreringsdatabasestierne for Office 2016 er ændret til 16,0. \Software\Microsoft\Office\16.0\Common\Identity\
- Angiv EnableADAL = 0 på den berørte computer ved hjælp af følgende trin:  
     1. Højreklik på Windows-knappen, og vælg **Kør**. Skriv **regedit**i feltet **Åbn** , og vælg derefter **OK**.
     2. Vælg **Ja,** når du bliver bedt om at tillade, at Registreringseditor foretager ændringer på enheden.
    3. Tilføj en DWORD-værdi for EnableADAL i Registreringseditor med en indstilling på 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Hvis fejlen opstår under oprettelse af forbindelse til Office 365 ved hjælp af Office 2013, skal du [aktivere moderne godkendelse](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) af Office-klienten.

Du kan finde flere oplysninger under [Sådan foretages fejlfinding af apps, der ikke er browsere, og som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

