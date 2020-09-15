---
title: Fejlfinding af synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664920"
---
# <a name="troubleshoot-password-synchronization"></a>Fejlfinding af synkronisering af adgangskoder

Hvis du vil udføre fejlfinding af problemer med synkronisering af adgangskoder, skal du starte med at bruge denne AAD-forbindelses fejlfindings opgave for at finde ud af, hvorfor adgangskoder ikke Gå til [Administrer direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)for at starte.  

1. Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren, og vælg indstillingen **Kør som administrator** .

2. Kør set-ExecutionPolicy RemoteSigned eller set-ExecutionPolicy ubegrænset.

3. Start guiden Azure AD Connect.

4. Gå til siden flere opgaver > **Foretag fejlfinding af**  >  **næste**.

5. Vælg **Start** for at åbne PowerShell-fejlfindings menuen.

6. Vælg **fejlfinding af adgangskode synkronisering**.

    Problemet er normalt, at en adgangskode ikke er synkroniseret for en bestemt brugerkonto.

    **Noter** Synkronisering af adgangskoder mislykkes, hvis den seneste vellykkede adgangskode synkronisering var et stykke tid siden.

Hvis du vil have mere hjælp til fejlfinding af adgangskode synkronisering, skal du se [fejlfinding af synkronisering af adgangskoder med Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).