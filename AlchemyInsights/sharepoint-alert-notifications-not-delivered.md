---
title: SharePoint-advarselsmeddelelser blev ikke leveret
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047061"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-advarselsmeddelelser blev ikke leveret

Tjek venligst JUNK mappen i din e-mail, som undertiden advarsler kan gå der.

Find ud af, om **alle påmindelser ikke er leveret** , eller om der ikke er leveret **en individuel besked** fra en specifik fil eller et bestemt bibliotek.

- **Individuelle påmindelser leveres ikke**: Hvis der ikke leveres en individuel besked fra en bestemt fil eller et specifikt bibliotek, kan du forsøge at slette og genskabe den. Se [administrere, få vist eller slette SharePoint-påmindelser](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) for at genskabe beskeden.
- **Alle påmindelser leveres ikke**: Hvis alle påmindelser fra flere filer eller biblioteker ikke leveres, skal du gå til [dashboardet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at kontrollere, om der er meddelelser/hændelser, som kan forekomme med SharePoint eller Exchange. Problemet kan være med SharePoint Alert kapacitet eller forsinkelser i e-mails via Exchange. Det vil også være vigtigt at bemærke, om andre e-mails bliver leveret, og hvis ikke, er problemet sandsynligvis med veksel forsinkelser.

Ofte stillede spørgsmål om påmindelser:

- Det er ikke muligt at sende påmindelser til distributionsgruppen, men kun sikkerheds-og O365-grupper understøttes.
- Du kan ikke tilpasse skabeloner til e-mail-beskeder. Du skal bruge Microsoft FLOW eller SharePoint Designer workflow for at opnå disse.

Flere oplysninger:

- **Besked opsætning**: du kan finde flere oplysninger om konfiguration af påmindelser under [oprette en besked om at få besked, når en fil eller mappe ændres i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Fejlfinding i forbindelse med påmindelser**: du kan finde flere oplysninger om fejlfinding af beskeder under [brugere modtager ikke meddelelser om SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Avancerede politikker for overholdelse af O365-regler**: du finder flere oplysninger om, hvordan du konfigurerer disse påmindelser, under [politikker for overholdelses](https://docs.microsoft.com/office365/securitycompliance/alert-policies)advarsler.
- **Overvågningslogfiler for SharePoint og OneDrive**: du finder flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Advarsler sendt af Advanced Threat Protection**: Se [ATP til SharePoint og OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Advarsler sendt af politikker for forebyggelse af**datatab: Se [e-MAILNOTIFIKATIONER for DLP-politik](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Relaterede emner

Vil du prøve Microsoft flow i SharePoint Online?

- [Opret flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint og flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
