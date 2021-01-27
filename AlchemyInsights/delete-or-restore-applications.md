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
# <a name="delete-or-restore-applications"></a><span data-ttu-id="2abb7-102">Slette eller gendanne programmer</span><span class="sxs-lookup"><span data-stu-id="2abb7-102">Delete or restore applications</span></span>

<span data-ttu-id="2abb7-103">**Sådan slettes et program fra Azure ad-lejeren**:</span><span class="sxs-lookup"><span data-stu-id="2abb7-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="2abb7-104">I **Azure ad-portalen** skal du vælge **virksomhedsprogrammer**.</span><span class="sxs-lookup"><span data-stu-id="2abb7-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="2abb7-105">Find og vælg derefter det program, du vil slette.</span><span class="sxs-lookup"><span data-stu-id="2abb7-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="2abb7-106">I sektionen **Administrer** i venstre rude skal du vælge **Egenskaber**.</span><span class="sxs-lookup"><span data-stu-id="2abb7-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="2abb7-107">Vælg **Slet**, og vælg derefter **Ja** for at bekræfte, at du vil slette APPEN fra din Azure ad-lejer.</span><span class="sxs-lookup"><span data-stu-id="2abb7-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="2abb7-108">Hvis du vil have mere at vide om, hvordan du sletter en app, skal du se under [hurtig start: Slet et program fra din Azure Active Directory-lejer (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="2abb7-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="2abb7-109">I PowerShell fjerner [Fjern-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) -cmdlet'en program proxy-konfigurationer fra et bestemt program i Azure Active Directory og kan slette programmet fuldstændigt, hvis det er angivet.</span><span class="sxs-lookup"><span data-stu-id="2abb7-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="2abb7-110">Du kan **gendanne et slettet program** ved hjælp af PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2abb7-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="2abb7-111">Når det program, du vil gendanne, er blevet identificeret, kan du gendanne det ved hjælp af [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="2abb7-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
