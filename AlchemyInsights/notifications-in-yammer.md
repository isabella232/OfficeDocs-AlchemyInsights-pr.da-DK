---
title: Meddelelser i Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662787"
---
# <a name="notifications-in-yammer"></a>Meddelelser i Yammer

For at advare brugerne om ny aktivitet i relevante samtaler, sender [Yammer meddelelser](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) enten via mail eller – for brugere med mobilenheder – gennem pushmeddelelser. Yammer sender som standard meddelelser for mange typer aktiviteter i dit netværk. Brugerne kan opdatere deres mailindstillinger via Yammer-webstedet, og pushmeddelelser konfigureres via mobilappen. 

Yammer har tilføjet understøttelse af [interaktive mails i Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Nogle mails (kopi af meddelelse) bliver interaktive i Outlook på internettet. En fremtidig opdatering vil føje dette til andre versioner af Outlook.

**Typer af meddelelser i Yammer**

- Mails (opdateringer fra en gruppe, en person inviterer dig til en gruppe, du modtager en besked i din indbakke osv.).
- Pushmeddelelser (sendt til mobilenheder, når du bliver nævnt, modtager en meddelelse i din indbakke osv.).
- Skrivebords-pop-op-vinduer (når du har installeret Yammer-skrivebordsappen, viser den meddelelser for brugere, der kaldes "toast"-meddelelser).
- Klokkemeddelelser (på Yammer-webstedet får brugerne vist meddelelser for forskellige hændelser. Disse meddelelser har muligvis ikke altid en tilknyttet mail- eller pushmeddelelse).

Du kan få mere [detaljerede oplysninger om meddelelser](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Administrering af meddelelser**

Brugerne skal administrere deres egne meddelelser. Du kan finde flere oplysninger om, [hvordan du kan aktivere og deaktivere Yammer mail- og mobilmeddelser](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Det er ikke muligt for administratorer at deaktivere alle meddelelser, eller styre meddelelser, på vegne af brugere. Administratorer kan [styre det logo, der er inkluderet i mails, og om brugerne skal bekræfte meddelelser](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer), der sendes via mail.

**Mailmeddelelser, der sendes til mange brugere i organisationen**

Nogle gange bliver der sendt en enkelt mailmeddelelse af Yammer, som modtages af mange flere brugere i din organisation end forventet. Dette sker, hvis en distributionsliste eller en anden type ikke-individuel mailadresse føjes til Yammer. Yammer kender ikke i alle tilfælde, om en mailadresse tilhører en enkelt bruger eller er en mailadresse, der medfører, at der sendes en mail til mange modtagere. Når dette problem opstår, skal du [suspendere (deaktivere) den ugyldige bruger med denne mailadresse](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) i Yammer. 

Hvis du vil mindske risikoen for, at dette problem opstår, skal du gøre følgende:

1. [Gennemtving Office 365-identitet](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) for Yammer.
2. Bloker eksterne afsendere fra at sende mails til din organisation, eller begræns afsendere til en godkendt liste.

Hvis dette problem opstår:

1. Identificer modtageren af mailen, som skal svare til brugeren i Yammer. All-in-sales@fabrikam.com er f.eks. en DL for alle sælgere. Denne DL vil kunne identificeres ud fra de Yammer-mails, der modtages af brugerne.
2. Brug funktionen [Deaktiver (suspender) i Netværksadministrator](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) til at suspendere brugeren, der har all-in-sales@fabrikam.com-mailadressen. Suspension kan fortrydes, så det er mere sikkert end sletning. Brugeren slettes automatisk efter 90 dage.
3. Du kan også gennemse [Brugereksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) for at finde andre ikke-brugerbaserede mailadresser, der skal suspenderes.
