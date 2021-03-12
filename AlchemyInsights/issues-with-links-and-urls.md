---
title: Problemer med links og URL-adresser
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707876"
---
# <a name="issues-with-links-and-urls"></a>Problemer med links og URL-adresser

Omdirigerings-URI'er/svar-URL-adresser (begge udtryk er synonyme) er de URL-adresser, der bruges af Microsoft-identitetsplatformen til at returnere tokens, der er forespurgt af en app. Du kan finde flere oplysninger om disse URL-adresser i følgende artikler:

- [Godkendelsesflows og programscenarier](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – oplysninger om omdirigerings-URI'er på siden **Appregistrering** for hvert scenarie.
- [Restriktioner og begrænsninger for omdirigerings-URI'er/svar-URL-adresser](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jeg ved ikke, hvordan jeg kan registrere den rigtige omdirigerings-URI/svar-URL-adresse til min app**

Når du logger på med det program, du udvikler, skal du, hvis logondialogboksen viser **AADSTS50011: Svar-URL-adressen i den angivne anmodning tilsvarer ikke svar-URL-adresserne, der er konfigureret for programmet <your app ID>**, føje omdirigerings-URI'en, som din kode brugte i tokenanmodningenen til Microsoft-identitetsplatformen, til din programanmodning.

Hvis du vil tilføje en svar-URL-adresse, skal du gå til fanen **Godkendelse** på din side til **programregistrering** i Azure-portalen og tilføje en post i sektionen **Omdirigerings-URI'er**. Den værdi, du angiver, afhænger af den type program, du bygger, som beskrevet nedenfor:

- I programmer og webapps med en side er svar-URL-adressen en URL-adresse i dit program. Se [Registrering af et program med én side](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) eller [Registrer en webapp med Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- For desktopapps afhænger den værdi, du skal vælge, af:
    - platformen (MacOS er forskellig fra Windows eller Linux)
    - den måde, du får din token på (interaktivt, med enhedskodeflow, med integreret Windows-godkendelse [IWA] eller med brugernavn/adgangskode).
    Du kan finde flere oplysninger i [Desktop-apps – Appregistrering – Omdirigerings-URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- For mobilprogrammer afhænger omdirigerings-URI'en af:
    - platformen (iOS/Android/UWP)
    - de oplysninger, der bruges til at udvikle din app, f.eks. bundle-id'et i iOS og pakkenavnet og signaturhashen på Android. Azure-portalens appregistrering hjælper dig. Du kan finde flere oplysninger i [Platformskonfiguration og omdirigerings-URI'er](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web-API'er og nogle af de diskrete måder at hente tokens på (IWA og brugernavn/adgangskode) kræver ikke noget omdirigerings-URI.

**Jeg har installeret mit webprogram, og når jeg tester den udrullede app, får jeg en besked om uoverensstemmelse for svar-URL-adressen**

Tilføj omdirigerings-URI'er for alle de placeringer, hvor du udruller dit webprogram. Du kan få flere oplysninger i [Registrer en webapp ved hjælp af Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Tilføj omdirigerings-URI'en for en placering, straks efter du har udrullet et program til den placering.

**Jeg kan ikke registrere tilstrækkeligt med svar-URL-adresser**

Du er en uafhængig softwareleverandør, og du har en eller flere omdirigerings-URI'er for hver af dine kunder. Du ønsker at migrere fra ADAL/Azure Active Directory v1.0 til MSAL/Microsoft-identitetsplatformen, og du har nået det [maksimale antal omdirigerings-URI'er](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Du kan løse dette problem ved at [tilføje omdirigerings-URI'er til de tjenesteprincipaler](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), der tilsvarer hver enkelt af dine kunder.
