---
title: Begrænsninger for følsomhedsetiketter for Office filer i SharePoint og OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813152"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Begrænsninger for følsomhedsetiketter for Office filer i SharePoint og OneDrive

Når du aktiverer følsomhedsetiketter for Office filer i SharePoint og OneDrive, skal du være opmærksom på krav og begrænsninger, som omfatter:

- SharePoint og OneDrive kan ikke behandle visse filer, der er mærket og krypteret fra Office-skrivebordsapps, når filerne indeholder PowerQuery-data, data gemt af brugerdefinerede tilføjelsesprogrammer eller brugerdefinerede XML-dele.
- SharePoint og OneDrive anvender ikke følsomhedsmærkater automatisk på eksisterende filer, du allerede har krypteret med Azure Information Protection-etiketter (AIP). Sådan anvender du følsomhedsmærkater på krypterede filer: 
    - Sørg for, at AIP-navne er blevet overført og publiceret i Microsoft 365 Compliance Center.
    - Download de mærkede filer, og upload dem derefter til deres oprindelige placering SharePoint eller OneDrive placering.
- For krypterede dokumenter understøttes udskrivning ikke.

Du kan finde flere oplysninger om begrænsninger [i Aktivér følsomhedsetiketter for Office filer i SharePoint og OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
