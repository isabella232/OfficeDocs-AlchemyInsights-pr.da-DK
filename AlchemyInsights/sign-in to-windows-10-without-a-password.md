---
title: Logge på Windows 10 uden at bruge en adgangskode
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719947"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logge på Windows 10 uden at bruge en adgangskode

Hvis du vil undgå at skulle skrive en adgangskode ved start af Windows, anbefaler vi, at du bruger en af de Secure-logonindstillinger til Windows Hello, som en pinkode, ansigtsgenkendelse eller fingeraftryk, hvis det er muligt. Hvis du er sikker på, at du vil deaktivere Secure logon, skal du se instruktionerne "Log automatisk på Windows 10" nedenfor.

**Sikre Windows Hello-alternativer til kontoens adgangskode**

Gå til **indstillinger > konti > indstillinger for logon** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgængelige logonindstillinger vises. Det kan f.eks. være:

![Logonindstillinger.](media/sign-in-options.png)

Klik eller tryk på en af indstillingerne for at konfigurere den. Næste gang du starter eller låser Windows op, kan du bruge den nye indstilling i stedet for en adgangskode. 

**Logge på Windows 10 automatisk**

**Bemærk**! det er praktisk at logge på automatisk logon, men det introducerer en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer. 

1. Klik eller tryk på knappen **Start** på proceslinjen.

2. Skriv **netplwiz** , og tryk på ENTER for at åbne vinduet brugerkonti.

3. I **brugerkonti**skal du klikke på den konto, du automatisk vil logge på, når Windows starter.

4. Fjern markeringen i afkrydsningsfeltet "brugerne skal angive et Brugernavn og en adgangskode for at bruge denne computer".

    ![Brugerne skal angive et Brugernavn og en adgangskode indstilling.](media/users-must-enter-username.png)

5. Klik på **OK**. Du bliver bedt om at angive og bekræfte adgangskoden for den konto, du har valgt. Klik på **OK** for at afslutte. Næste gang Windows 10 starter, bliver den automatisk logget på den konto, du har valgt.
