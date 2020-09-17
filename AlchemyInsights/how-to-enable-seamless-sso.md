---
title: Sådan aktiveres problemfrit SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780521"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="f8d03-102">Sådan aktiveres problemfrit SSO</span><span class="sxs-lookup"><span data-stu-id="f8d03-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="f8d03-103">Aktivér problemfrit SSO via [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="f8d03-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="f8d03-104">Hvis du foretager en ny installation af Azure AD Connect, skal du vælge den [brugerdefinerede](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)installationssti.</span><span class="sxs-lookup"><span data-stu-id="f8d03-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="f8d03-105">På logonsiden til **brugere** skal du vælge indstillingen **Aktivér enkeltlogon** .</span><span class="sxs-lookup"><span data-stu-id="f8d03-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="f8d03-106">Sådan kontrollerer du, at du har aktiveret problemfrit SSO korrekt:</span><span class="sxs-lookup"><span data-stu-id="f8d03-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="f8d03-107">Log på [Azure Active Directory administration](https://aad.portal.azure.com) som global administrator.</span><span class="sxs-lookup"><span data-stu-id="f8d03-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="f8d03-108">Vælg **Azure Active Directory** i venstre rude.</span><span class="sxs-lookup"><span data-stu-id="f8d03-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="f8d03-109">Kontrollér, at problemfrit enkeltlogon er **aktiveret**.</span><span class="sxs-lookup"><span data-stu-id="f8d03-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="f8d03-110">Hvis du vil have mere at vide, skal du se [Azure Active Directory problemfrit enkeltlogon: hurtig start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="f8d03-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  