---
title: Teams almindelige problemer for Education-kunder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: d61d4484c720db51e7377201067008192940d1f8
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43739430"
---
# <a name="teams-common-issues-for-education-customers"></a>Teams almindelige problemer for Education-kunder

**Til uddannelseskunder**:

Hvis du har brug for hjælp til at anvende Teams til at understøtte ekstern læring, skal du gå til [FastTrack Center](https://www.microsoft.com/fasttrack) for at sende en anmodning. Se følgende almindelige problemer for Teams Education-kunder:

- Får de vist meddelelsen "**Der er noget, du går glip af!**"? Sørg for at [aktivere Microsoft Teams for din skole](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). I EDU-lejere er Microsoft Teams ikke aktiveret som standard. Du skal først slå det til.

- **Er du ny bruger af Teams?** Gennemse [Fjernundervisning og læring i Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) for at se den mest opdaterede vejledning i, hvordan du konfigurerer din skole, planlægning af lektioner, virtuelle møder og deling af indhold med studerende.

- Når den er slået til, kan brugerne køre Teams ved enten at installere [stationære](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) og [bærbare klienter](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) eller fra browseren på https://teams.microsoft.com.

- **Aktivér Teams-gæsteadgang**: Gennemse [tjeklisten for Teams-gæsteadgang](https://docs.microsoft.com/microsoftteams/guest-access-checklist), og sørg for, at alle trin er fuldført.
    - [Forstå gæsteadgang i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Konfiguration – kontrolliste til gæsteadgang for Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Hvordan en gæst tilmelder sig et Team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-møder og opkald**: Har du brug for hjælp til at aktivere eller konfigurere Lydmøde i Microsoft Teams? Er denne bruger blevet oprettet for nylig? Hvis det er tilfældet, skal du vente i 2-24 timer, før ændringerne træder i kraft. Sådan bekræfter du, at brugeren er licenseret til lydmøder og har et standard afgiftsbelagt nummer:
    1. Gå til Aktive brugere, og vælg den pågældende bruger.
    2. Afhængigt af din version af administrationscenteret skal du vælge enten **Licenser og apps** eller klikke på **Rediger** på **Produktlicenser**.
    3. Bekræft, at brugeren har licenserne, der er valgt til Lydmøde, Microsoft Teams og Skype for Business online (Plan 2).
    4. I Administrationscentre skal du klikke på **Vis alle** og derefter **Teams**.
    5. I Microsoft Teams Administration skal du klikke på **Gammel portal**.
    6. I Skype for Business Administration skal du klikke på **Lydmøde** og derefter på **Brugere**.
    7. Vælg den pågældende bruger, og bekræft, at brugeren har et standard afgiftsbelagt nummer.

    Du kan finde flere oplysninger under [Opkaldsabonnementer](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) eller ringe til Microsoft Commerce-faktureringsteamet for at få hjælp til licensrelaterede spørgsmål.

    Flere ressourcer

    - [Møder og konferencer i Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Lydmøde](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Mødepolitikker**: Mødepolitikker bruges til at styre de funktioner, der er tilgængelige for mødedeltagere for møder, der er planlagt af brugerne i din organisation. Efter du har oprettet en politik og gennemført dine ændringer, kan du tildele brugere til politikken.

    - **Rediger eller opret en mødepolitik**: Hvis du vil ændre eller oprette en mødepolitik, skal du gå til **Microsoft Teams Administration > Møder > Mødepolitikker**.  Vælg en politik fra listen eller klik på **Tilføj**. Hvis du opretter en ny politik, skal du tilføje et navn og en beskrivelse. Navnet må ikke indeholde specialtegn eller være længere end 64 tegn. Vælg dine indstillinger, og klik derefter på **Gem**. 
    
        Lad os f.eks. sige, at du har en masse brugere, og du vil begrænse den båndbredde, som deres møde kræver. Du skal oprette en ny brugerdefineret politik kaldet "begrænset båndbredde" og deaktivere de følgende indstillinger:

        Under **lyd og video**:
        - Deaktiver **Tillad optagelse i skyen**.
        - Deaktiver **Tillad IP-video**.

        Under **Deling af indhold**:

        - Deaktiver skærmdelingstilstand.
        - Deaktiver **Tillad whiteboard**.
        - Deaktiver **Tillad delte noter**.

        Tildel derefter**politikken til brugerne**:

    1. I venstre navigationsrude i Microsoft Teams Administration skal du gå til **Brugere **og derefter klikke på brugeren.
    2. Markér brugeren ved at klikke til venstre for brugernavnet, og klik derefter på **Rediger indstillinger**.
    3. Under **Mødepolitik** skal du markere den politik, du vil tildele, og derefter klikke på **Tildel**. 

    Hvis du vil tildele en politik til flere brugere ad gangen, skal du se [Rediger indstillinger for Teams-brugere i bulk](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Eller du kan gøre følgende:
    1. I venstre navigationsrude i Microsoft Teams Administration skal du gå til **Møder > Mødepolitikker**.
    2. Vælg politikken ved at klikke til venstre for politikkens navn.
    3. Klik på **Administrer brugere**.
    4. I ruden **Administrer brugere** skal du søge efter brugeren med det viste navn eller brugernavnet, vælge navnet og derefter klikke på **Tilføj**. Gentag dette trin for hver bruger, du vil tilføje.
    5. Når du er færdig med at tilføje brugere, skal du klikke på **Gem**.

- **Fejlfinding i forbindelse med manglende numerisk tastatur**:
    - Sørg for, at brugeren er tildelt en [Teams-licens](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Sørg for, at brugeren er tildelt et [opkaldsabonnement](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Aktivér brugerne til [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Fejlfinding af Teams-logon**: Du skal først sikre dig, at [tjenesten Microsoft Teams er i god stand](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Kontrollér derefter, om der er almindelige fejlkoder, og gennemse [Hvorfor har jeg problemer med at logge på Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)? Du skal muligvis også gennemse [Identitetsmodeller og godkendelse i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
