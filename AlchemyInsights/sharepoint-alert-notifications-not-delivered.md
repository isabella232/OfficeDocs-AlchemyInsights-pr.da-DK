---
title: Meddelelser om SharePoint-beskeder er ikke leveret
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742041"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Meddelelser om SharePoint-beskeder er ikke leveret

Kontroller mappen UØNSKET mail i din mail, da der nogle gange kan gå advarsler derhen.

Find ud af, om **alle beskeder ikke leveres,** eller om **en individuel besked** fra en bestemt fil eller et bestemt bibliotek ikke leveres.

- **Individuelle beskeder leveres ikke**: Hvis en individuel besked fra en bestemt fil eller et bestemt bibliotek ikke leveres, kan du forsøge at slette og genoprette den. Se [Administrere, få vist eller slette SharePoint-beskeder](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for at genoprette beskeden.
- **Alle beskeder leveres ikke:** Hvis alle beskeder fra flere filer eller biblioteker ikke leveres, skal du gå til [dashboardet Tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at søge efter eventuelle meddelelser/hændelser, der kan forekomme med SharePoint eller Exchange. Problemet kan være med SharePoint-beskedfunktionen eller forsinkelser i e-mails via Exchange. Det vil også være vigtigt at bemærke, om andre e-mails bliver leveret, og hvis ikke, er problemet sandsynligvis med Forsinkelser i Exchange.

Ofte stillede spørgsmål om advarsler:

- Det er ikke muligt at sende beskeder til distributionsgruppen, kun sikkerheds- og O365-grupper understøttes.
- Du kan ikke tilpasse mailskabeloner til påmindelser. Du skal bruge Microsoft FLOW eller SharePoint Designer Workflow for at opnå disse.

Flere oplysninger:

- **Konfiguration af beskeder**: Du kan finde flere oplysninger om konfiguration af beskeder under [Oprette en besked for at få besked, når en fil eller mappe ændres i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Fejlfinding af beskeder**: Du kan finde flere oplysninger om fejlfinding af advarsler under [Brugere modtager ikke Meddelelser om Beskeder om SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Avancerede O365-politikker for overholdelse af regler og standarder**: Du kan finde flere oplysninger om konfiguration af disse påmindelser under Politikker for overholdelse af regler for overholdelse af regler for [overholdelse](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **SharePoint- og OneDrive-overvågningslogfiler**: Du kan finde flere oplysninger om, hvordan du henter disse hændelser, [under Søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Beskeder, der sendes af Avanceret trusselsbeskyttelse:** Se [ATP for SharePoint og OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Advarsler sendt af datatab forebyggelse politikker**: Se [E-mail-meddelelser for DLP politikker](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Relaterede emner

Vil du prøve Microsoft Flow i SharePoint Online?

- [Opret flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint og Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
