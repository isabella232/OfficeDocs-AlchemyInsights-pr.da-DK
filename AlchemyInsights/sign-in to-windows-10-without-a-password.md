---
title: Log på Windows 10 uden at bruge en adgangskode
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830540"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Log på Windows 10 uden at bruge en adgangskode

For at undgå at skulle skrive en adgangskode ved start af Windows anbefaler vi, at du bruger en af Windows Hello-indstillingerne til sikker logon, f.eks. en pinkode, ansigtsgenkendelse eller fingeraftryk, hvis den er tilgængelig. Hvis du er sikker på, at du vil deaktivere sikker logon, skal du se vejledningen "Log automatisk på Windows 10" nedenfor.

**Gør Windows Hello-alternativer sikre til adgangskoden til kontoen**

Gå til **Indstillinger > konti > Logonindstillinger** (eller klik [her).](ms-settings:signinoptions?activationSource=GetHelp) De tilgængelige indstillinger for logon vises. Eksempel:

![Logonindstillinger.](media/sign-in-options.png)

Klik eller tryk på en af indstillingerne for at konfigurere den. Næste gang du starter eller låser Windows op, vil du kunne bruge den nye indstilling i stedet for en adgangskode. 

**Log automatisk på Windows 10**

**Bemærk!** Automatisk logon er praktisk, men introducerer en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer. 

1. Klik eller tryk på **knappen Start** på proceslinjen.

2. Skriv **netplwiz,** og tryk på Enter for at åbne vinduet Brugerkonti.

3. Under **Brugerkonti skal** du klikke på den konto, du automatisk vil logge på, når Windows starter.

4. Fjern markeringen i afkrydsningsfeltet "Brugere skal angive et brugernavn og en adgangskode for at bruge denne computer".

    ![Brugere skal angive et brugernavn og en adgangskode.](media/users-must-enter-username.png)

5. Klik på **OK**. Du bliver bedt om at angive og bekræfte adgangskoden for den konto, du har valgt. Klik **på OK** for at afslutte. Næste gang Windows 10 starter, logges der automatisk på den konto, du har valgt.
