---
title: Problemer med links og URL-adresser
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974301"
---
# <a name="issues-with-links-and-urls"></a>Problemer med links og URL-adresser

Omdirigering af URI/svar-URL-adresser (begge udtryk kan erstattes) er de URL-adresser, der bruges af Microsoft Identity platform til at returnere app-anmodede tokens. Hvis du vil have mere at vide om disse URL-adresser, skal du se følgende artikler:

- [Godkendelses flow og programscenarier](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – oplysninger om omdirigerings-URI'erne på siden **app Registration** for hvert scenarie.
- [URL-begrænsninger og-begrænsninger for omdirigering af URI/svar](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jeg ved ikke, hvordan jeg registrerer URL-adressen til højre omdirigering for min app**

Når du logger på med det program, du udvikler, skal du, hvis dialogboksen til logon viser **AADSTS50011: den URL-adresse for svar, der er angivet i anmodningen, ikke stemmer <your app ID> overens med URL-adresserne for det program, der er konfigureret for programmet**, skal du tilføje den omdirigerings URI, som din kode har brugt i anmodningen om token, til Microsoft Identity platform.

Hvis du vil tilføje en svar-URL-adresse, skal du gå til fanen **godkendelse** på din **program registrerings** side i Azure-portalen og tilføje en post i sektionen **Redirect URI'er** . Omdirigerings-URI'er skrives (Web eller mobile/computer). Den værdi, du skal angive, afhænger af den type program, du er ved at opbygge, som beskrevet nedenfor:

- For enkeltsidede programmer og web apps er svar-URL-adressen en URL-adresse i dit program. Se en [enkeltsidet programregistrering](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) eller [registrere en Web App-app ved hjælp af Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- For skrivebordsapps er det den værdi, du skal vælge, afhænger af:
    - platformen (MacOS er forskellig fra Windows eller Linux)
    - den måde, du køber tokenet på (interaktivt med Enhedskode strøm, med integreret Windows-godkendelse [IWA] eller med brugernavn/adgangskode).
    Hvis du vil have mere at vide, skal du se [skrivebordsapps – registrering af app-omdirigering-URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- For mobilprogrammer afhænger omdirigerings URI'EN af:
    - platformen (iOS/Android/UWP)
    - de oplysninger, der bruges til at opbygge din app, såsom Bundle-id'et i iOS, og pakkens navn og signatur hash på Android-App til Azure-portalen vil hjælpe dig. Du kan få mere at vide under [platform konfiguration og omdirigering af URI'er](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Webapi'erne og nogle af de bestillende metoder til at hente tokens (IWA og brugernavn/adgangskode) kræver ikke en omdirigerings URI.

**Jeg har installeret mit webprogram, og når jeg tester den installerede app, får jeg en meddelelse om uoverensstemmelse for svar URL**

Tilføj omdirigerings URI'er for alle de placeringer, hvor du installerer dit webprogram. Du kan finde flere oplysninger i afsnittet [registrere en Web App-app ved hjælp af Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Tilføj omdirigerings-URI for en placering, umiddelbart efter at du har installeret programmet på den placering.

**Jeg kan ikke registrere nok svar-URL-adresser**

Du er ISV og har en eller flere omdirigerings-URI'er til hver kunde. Du vil overføre fra ADAL/Azure AD v 1.0 til MSAL/Microsoft Identity platform, og du støder på det [maksimale antal omdirigerings URI'er](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Du kan løse dette problem ved at [tilføje omdirigerings-URI'er til service konti](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , der svarer til hver af dine kunder.
