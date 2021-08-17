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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105742"
---
# <a name="troubleshoot-password-synchronization"></a>Fejlfinding af synkronisering af adgangskoder

Hvis du vil foretage fejlfinding af problemer med synkronisering af adgangskoder, skal du starte med at bruge denne AAD Forbind fejlfinding til at finde ud af, hvorfor adgangskoder ikke synkroniseres. For at komme i gang skal du [gå til Administrer direkte synkronisering.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Åbn en ny Windows PowerShell på Azure AD Forbind-serveren, og vælg **indstillingen Kør som** administrator.

2. Kør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Ubegrænset.

3. Start Azure AD Forbind guiden.

4. Gå til siden Yderligere opgaver, og > **Næste.**  >  

5. Vælg **Start** for at åbne PowerShell-fejlfindingsmenuen.

6. Vælg Fejlfinding **i forbindelse med synkronisering af adgangskoder.**

    Problemet er som regel, at en adgangskode ikke er synkroniseret for en bestemt brugerkonto.

    **Noter** Synkronisering af adgangskoder mislykkes, hvis det sidste fuldførte synkronisering af adgangskoder var for et stykke tid siden.

Du kan få mere hjælp til fejlfinding i forbindelse med synkronisering af adgangskoder [under Fejlfinding af synkronisering af adgangskodehash med Azure AD Forbind synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)