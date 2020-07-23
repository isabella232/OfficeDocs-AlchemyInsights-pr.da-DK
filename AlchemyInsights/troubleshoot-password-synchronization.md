---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387871"
---
# <a name="troubleshoot-password-synchronization"></a>Fejlfinding i forbindelse med synkronisering af adgangskoder

Hvis du vil foretage fejlfinding af problemer med synkronisering af adgangskoder, skal du starte med at bruge denne fejlfindingsopgave til AAD Connect for at finde ud af, hvorfor adgangskoder ikke synkroniseres. Gå til Administrer direkte [synkronisering for at begynde.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Åbn en ny Windows PowerShell-session på din Azure AD Connect-server, og vælg **indstillingen Kør som** administrator.

2. Kør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Unrestricted.

3. Start guiden Azure AD Connect.

4. Gå til siden Yderligere opgaver > **Fejlfinding af**  >  **næste**.

5. Vælg **Start** for at åbne fejlfindingsmenuen i PowerShell.

6. Vælg **Fejlfinding af synkronisering af adgangskode**.

    Problemet er normalt, at en adgangskode ikke synkroniseres for en bestemt brugerkonto.

    **Bemærkninger** Synkronisering af adgangskoder mislykkes, hvis den seneste vellykkede synkronisering af adgangskoder var for nogen tid siden.

Du kan finde flere hjælp til fejlfinding af synkronisering af adgangskoder under [Fejlfinding af synkronisering af hash for adgangskoder med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).