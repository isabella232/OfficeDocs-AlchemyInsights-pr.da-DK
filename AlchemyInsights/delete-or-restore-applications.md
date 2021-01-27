---
title: Slette eller gendanne programmer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014797"
---
# <a name="delete-or-restore-applications"></a>Slette eller gendanne programmer

**Sådan slettes et program fra Azure ad-lejeren**:

1. I **Azure ad-portalen** skal du vælge **virksomhedsprogrammer**. Find og vælg derefter det program, du vil slette.
2. I sektionen **Administrer** i venstre rude skal du vælge **Egenskaber**.
3. Vælg **Slet**, og vælg derefter **Ja** for at bekræfte, at du vil slette APPEN fra din Azure ad-lejer.

Hvis du vil have mere at vide om, hvordan du sletter en app, skal du se under [hurtig start: Slet et program fra din Azure Active Directory-lejer (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

I PowerShell fjerner [Fjern-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) -cmdlet'en program proxy-konfigurationer fra et bestemt program i Azure Active Directory og kan slette programmet fuldstændigt, hvis det er angivet.

Du kan **gendanne et slettet program** ved hjælp af PowerShell. Når det program, du vil gendanne, er blevet identificeret, kan du gendanne det ved hjælp af [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
