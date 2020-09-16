---
title: Oprette en organisations relation for at give brugerne mulighed for at samarbejde med en anden organisation
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
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712727"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>Oprette en organisations relation for at give brugerne mulighed for at samarbejde med en anden organisation

1. Fra Microsoft 365 administration-dashboardet skal du gå til **admin**  >  **Exchange**.
2. Gå til **organization**  >  **deling**af organisationer.
3. Klik på **ny** under **deling af organisation**.
4. I den **nye organisations relation**skal du skrive et brugervenligt navn for organisationens relation i feltet **Relationsnavn** .
5. I feltet **domæner, der skal deles med** skal du skrive domænet for den eksterne Office 365-eller Exchange lokalt-organisation, du vil give dig mulighed for at se dine kalendere. Hvis du har brug for at angive mere end ét domæne, skal du adskille domænenavnene med et komma. For eksempel contoso.com, service.contoso.com.
6. Markér afkrydsningsfeltet **Aktivér deling af oplysninger om ledig/optaget-kalender** for at aktivere kalender deling med de domæner, du har angivet. Angiv delings niveauet for oplysninger om ledig/optaget tid i kalenderen, og Angiv, hvilke brugere der kan dele kalenderoplysninger om ledig/optaget tid.  

Hvis du vil angive adgangsniveauet ledig/optaget, skal du vælge en af følgende:

- **Oplysninger om ledig/optaget tid i kalenderen**
- **Kalender ledig/optaget til tid, emne og placering**  

 Hvis du vil angive, hvilke brugere der skal dele kalenderoplysninger om ledig/optaget tid, skal du vælge en af følgende:

- **Alle i organisationen**
- **En angivet sikkerhedsgruppe**  

Klik på **Gennemse** for at vælge sikkerhedsgruppen fra en liste, og klik derefter på **OK**.

Klik på **Gem** for at oprette organisations relationen.  

**Bemærk:** Konfigurationer på tværs af flere arkitekturer understøtter ikke personlige kontakter til opslag i ledig/optaget tid. Kontaktpersoner skal medtages på den globale adresseliste, hvor opslag i ledig/optaget tid fungerer.

**Hvis du vil have mere at vide om dette emne, skal du læse:**

- [Oprette en organisations relation i Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [Ændre en organisations relation i Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [Fjerne en organisations relation i Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
