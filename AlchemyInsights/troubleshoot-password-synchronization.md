---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732504"
---
# <a name="troubleshoot-password-synchronization"></a>Fejlfinding i forbindelse med synkronisering af adgangskoder

Sådan foretager du fejlfinding af problemer, hvor der ikke synkroniseres adgangskoder med Azure AD Connect version 1.1.614.0 eller nyere:
  
1. Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren med indstillingen **Kør som administrator.**

2. Kør **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy Ubegrænset**.

3. Start guiden Azure AD Connect.

4. Gå til siden **Flere opgaver,** vælg **Fejlfinding**, og klik på **Næste**.

5. Klik på Start på siden Fejlfinding **for at starte fejlfindingsmenuen** i PowerShell.

6. Vælg Fejlfinding af **synkronisering af adgangskoder i**hovedmenuen .

7. I undermenuen skal du vælge **Password Synkronisering virker slet ikke**.

**Forstå resultaterne af fejlfindingsopgaven**
  
Fejlfindingsopgaven udfører følgende kontroller:
  
- Validerer, at funktionen til synkronisering af adgangskoder er aktiveret for din Azure AD-lejer.

- Kontrollerer, at Azure AD Connect-serveren ikke er i midlertidig tilstand.

- For hver eksisterende Active Directory-forbindelse i det lokale miljø (hvilket svarer til et eksisterende Active Directory-område):

- 
  - Kontrollerer, at funktionen til synkronisering af adgangskoder er aktiveret.

  - Søger efter hjertestartere til synkronisering af adgangskoder i Windows Application Event-logfilerne.

  - For hvert Active Directory-domæne under den lokale Active Directory-forbindelse:

  - Validerer, at domænet kan nås fra Azure AD Connect-serveren.

  - Kontrollerer, at de AD DS-konti (Active Directory Domain Services), der bruges af det lokale Active Directory-stik, har det korrekte brugernavn, den korrekte adgangskode og de tilladelser, der kræves til synkronisering af adgangskoder.

Du kan få mere hjælp til fejlfinding af synkronisering af adgangskoder [under Fejlfinding af synkronisering af adgangskoder med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  