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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102565"
---
# <a name="delete-or-restore-applications"></a>Slette eller gendanne programmer

**Sådan sletter du et program fra din Azure AD-lejer:**

1. I **Azure AD-portalen skal** du vælge **Enterprise-programmer**. Find og vælg derefter det program, du vil slette.
2. I sektionen **Administrer** i venstre rude skal du vælge **Egenskaber**.
3. Vælg **Slet**, og vælg derefter **Ja for** at bekræfte, at du vil slette appen fra din Azure AD-lejer.

Du kan finde flere oplysninger om, hvordan du sletter en app, under Hurtig start: Slet et program fra din [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

I PowerShell fjerner cmdlet'en [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) programproxykonfigurationer fra et bestemt program i Azure Active Directory og kan slette programmet helt, hvis det er angivet.

Du kan **gendanne et slettet program ved hjælp** af PowerShell. Når det program, du vil gendanne, er blevet identificeret, kan du gendanne det ved hjælp [af Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
