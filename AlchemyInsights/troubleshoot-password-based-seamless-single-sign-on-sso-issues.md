---
title: Fejlfinding af adgangskodebaserede problemer med enkelt logon (Seamless Single Sign-on)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714709"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="36464-102">Fejlfinding af adgangskodebaserede problemer med enkelt logon (Seamless Single Sign-on)</span><span class="sxs-lookup"><span data-stu-id="36464-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="36464-103">Du kan få mere at vide om det grundlæggende ved adgangskodebaseret SSO [under Adgangskodebaseret godkendelse med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="36464-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="36464-104">**Konfigurere adgangskodebaseret SSO**</span><span class="sxs-lookup"><span data-stu-id="36464-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="36464-105">[Konfigurer adgangskodebaseret enkelt-logon – Denne](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) artikel indeholder flere oplysninger om den adgangskodebaserede SSO-indstilling.</span><span class="sxs-lookup"><span data-stu-id="36464-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="36464-106">Hvis det program, du tilføjer, kræver brugerdefineret konfiguration, og du skal bruge adgangskodebaseret SSO, er denne artikel for dig.</span><span class="sxs-lookup"><span data-stu-id="36464-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="36464-107">[Konfigurer adgangskodebaseret enkelttegn til apps i det pågældende program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy understøtter flere tilstande til enkelt logon.</span><span class="sxs-lookup"><span data-stu-id="36464-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="36464-108">Adgangskodebaseret logon er beregnet til programmer, der bruger en kombination af brugernavn/adgangskode til godkendelse.</span><span class="sxs-lookup"><span data-stu-id="36464-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="36464-109">Når du konfigurerer adgangskodebaseret logon til dit program, skal brugerne logge på det lokale program én gang.</span><span class="sxs-lookup"><span data-stu-id="36464-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="36464-110">Derefter gemmer Azure Active Directory logonoplysningerne og leverer dem automatisk til programmet, når dine brugere får adgang til dem eksternt.</span><span class="sxs-lookup"><span data-stu-id="36464-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="36464-111">Du bør allerede have publiceret og testet din app med programproxy.</span><span class="sxs-lookup"><span data-stu-id="36464-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="36464-112">Hvis ikke, skal du følge trinnene i Publicer programmer ved hjælp af Azure AD-programproxy og derefter fortsætte din konfiguration af adgangskodebaseret SSO til apps i det pågældende program. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)</span><span class="sxs-lookup"><span data-stu-id="36464-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="36464-113">Hvis du vil foretage fejlfinding af adgangskodebaseret SSO, skal du [se Fejlfinding af adgangskodebaseret enkelt logon i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="36464-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
