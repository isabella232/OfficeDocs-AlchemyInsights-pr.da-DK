---
title: Log på for at Windows 10 uden at bruge en adgangskode
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107502"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Log på for at Windows 10 uden at bruge en adgangskode

For at undgå at skulle skrive en adgangskode ved Windows opstart anbefaler vi, at du bruger en af de Windows Hello sikre logonindstillinger, f.eks. en pinkode, ansigtsgenkendelse eller fingeraftryk, hvis det er tilgængeligt. Hvis du er sikker på, at du vil deaktivere sikker logon, kan du se instruktionerne "Log automatisk på Windows 10" nedenfor.

**Sikre Windows Hello alternativer til adgangskoden til kontoen**

Gå til **Indstillinger > konti > logonindstillinger** (eller klik [her).](ms-settings:signinoptions?activationSource=GetHelp) De tilgængelige indstillinger for logon vises. Eksempel:

![Logonindstillinger.](media/sign-in-options.png)

Klik eller tryk på en af indstillingerne for at konfigurere den. Næste gang du starter eller Windows adgangskode, kan du bruge den nye indstilling i stedet for en adgangskode. 

**Log automatisk på Windows 10**

**Bemærk!** Automatisk logon er praktisk, men introducerer en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer. 

1. Klik eller tryk på **knappen Start** på proceslinjen.

2. Skriv **netplwiz,** og tryk på Enter for at åbne vinduet Brugerkonti.

3. Under **Brugerkonti skal** du klikke på den konto, du vil logge på automatisk, når Windows starter.

4. Fjern markeringen i afkrydsningsfeltet "Brugere skal angive et brugernavn og en adgangskode for at bruge denne computer".

    ![Brugere skal angive et brugernavn og en adgangskode.](media/users-must-enter-username.png)

5. Klik på **OK**. Du bliver bedt om at angive og bekræfte adgangskoden for den konto, du har valgt. Klik **på OK** for at afslutte. Næste gang Windows 10, logges der automatisk på den konto, du har valgt.
