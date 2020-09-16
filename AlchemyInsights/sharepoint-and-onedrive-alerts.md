---
title: Forsinkelser i modtagelse af SharePoint-og OneDrive-beskeder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727237"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Forsinkelser i modtagelse af SharePoint-og OneDrive-beskeder

- Kontrollér først mappen uønsket mail eller spam i din mail.
- Hvis **alle beskeder fra flere filer eller biblioteker forsinkes**, skal du gå til [tjeneste tilstands dashboardet](https://portal.office.com/adminportal/home?ref=/servicehealth) for at kontrollere, om der er nogen rådgivere/Incidents, der kan forekomme i SharePoint eller Exchange. Problemet kan skyldes SharePoint-beskedfunktionen eller-forsinkelser i mails via Exchange. Bemærk også, om der leveres andre mails – hvis ikke, er problemet sandsynligt med Exchange-forsinkelser.
- Hvis **en individuel besked fra en bestemt fil eller et bestemt bibliotek ikke er leveret**, skal du forsøge at slette og gendanne den. Se [Administrer, få vist eller Slet SharePoint-beskeder](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for at genoprette beskeden.

> [!NOTE]
> - Der kan ikke sendes beskeder til en distributionsgruppe. Kun sikkerheds-og O365-grupper understøttes.
> - Du kan ikke tilpasse mailskabeloner til påmindelser. Du skal bruge Microsoft flow-eller SharePoint Designer-arbejdsproces for at opnå dem.
