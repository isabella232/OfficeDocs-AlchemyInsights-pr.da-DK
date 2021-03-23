---
title: Problemer med brugeradministration
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035529"
---
# <a name="user-management-issues"></a>Problemer med brugeradministration

**Hvad sker der med aktuelle tildelte brugere til programmet, hvis jeg deaktiverer egenskaben "Brugertildeling påkrævet" (angiv denne egenskab til Nej)?**

Deaktivering **af brugertildeling påkrævet** påvirker IKKE de aktuelt tildelte brugere. Deaktivering af denne egenskab tillader kun alle brugere at få adgang til programmet. Alle de viste brugere og de brugere, der er tildelt grupper i programmet, vil stadig være gyldige.

- Hvis du vil begrænse din app til bestemte brugere, skal du se : Begræns Azure AD-appen til en række brugere [– Microsoft-identitetsplatformen | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- Hvis du vil tildele brugere og grupper til virksomhedsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjælp af PowerShell, skal du se Administrer brugertildeling for en app i [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Hvis du vil uddelegere tilladelser til oprettelse og administration af programmer, skal du se Stedfortrædertilladelser til [programadministration – Azure AD-| Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **Skjul bestemte virksomhedsapps for brugere** – Brug følgende trin til at skjule alle Microsoft 365-apps **fra panelet MyApps.** Appsene vil stadig være synlige på Office 365-portalen.

 1. Log på Azure-portalen som global administrator for dit katalog. 
 2. Vælg **Azure Active Directory.** 
 3. Vælg **Brugere.** 
 4. Vælg **Brugerindstillinger.** 
 5. Under **Virksomhedsprogrammer skal** du klikke **på Administrer, hvordan slutbrugere starter og får vist deres programmer.** 
 6. For **brugere kan kun se Office 365-apps i Office 365-portalen** skal du klikke på **Ja.** 
 7. Klik på **Gem**. 
 8. Få mere at vide under [Skjul et Enterprise-program fra brugerens oplevelse i Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Hvis du tilbyder en SaaS-app (Software as a Service) til mange organisationer, kan du konfigurere din app til at acceptere logons fra alle Azure Active Directory-lejere (Azure AD). Denne konfiguration kaldes "gør dit program til flere lejere". Brugere i alle Azure AD-lejere vil kunne logge på din app, når de har accepteret at bruge deres konto med din app. Få mere at vide under [Opbyg apps, der logger på Azure AD-brugere – Microsoft-identitetsplatformen | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **Hvordan kan en slutbruger få adgang til programmet, når han/hun er tildelt til programmet?**

Hver app i Enterprise-program bladet har et link, som slutbrugere kan få adgang til. Brugere kan også få adgang til appen **via Myapps-portalen** på en nem måde.

- **Vil du gerne vide, hvilke programmer og programtyper brugerne bruger?**

Du kan hente logonrapporter for de seneste 30 dage fra portal.azure.com > Azure Active Directory> **Signins> overførselsrapporter.**

- Få mere at vide [om, hvordan du giver administratorsamtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for hele lejeren og [konfigurerer slutbrugernes samtykke til programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Forstå, [hvordan samtykke fungerer,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [og Administrer samtykke til programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


