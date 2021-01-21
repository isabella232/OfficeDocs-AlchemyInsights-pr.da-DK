---
title: Konfigurere og udvide levetid for tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916732"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="d1f51-102">Konfigurere og udvide levetid for tokens</span><span class="sxs-lookup"><span data-stu-id="d1f51-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="d1f51-103">Du kan angive levetiden for en Access-, SAML-eller ID-token, der er udstedt af Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="d1f51-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="d1f51-104">Du kan angive levetiden for tokens for alle apps i organisationen, for et program med flere arkitekturer (flere virksomheder) eller for en bestemt tjeneste Principal i organisationen.</span><span class="sxs-lookup"><span data-stu-id="d1f51-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="d1f51-105">Du kan få mere at vide ved at læse [levetid for konfigurerbare tokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="d1f51-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="d1f51-106">For eksempler kan [du læse eksempler på, hvordan du konfigurerer levetid for tokens](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="d1f51-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="d1f51-107">Du kan få mere at vide om, hvordan du konfigurerer levetiden og kompatibiliteten af et token i Azure Active Directory B2C (Azure AD B2C) i [konfigurere tokens i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="d1f51-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="d1f51-108">Artiklen [konfigurere sessions funktionsmåde i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskriver de enkeltlogon-metoder (SSO), der bruges i Azure ad B2C og hjælper dig med at vælge den mest relevante SSO-metode, når du konfigurerer din politik.</span><span class="sxs-lookup"><span data-stu-id="d1f51-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="d1f51-109">**Hvor lang tid er tokens sidst? Hvor lang tid gælder de for?**</span><span class="sxs-lookup"><span data-stu-id="d1f51-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="d1f51-110">Levetid for tokens er 1 time, og sessionens levetid er 24 timer.</span><span class="sxs-lookup"><span data-stu-id="d1f51-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="d1f51-111">Det betyder, at hvis der ikke er foretaget nogen anmodninger inden for 24 timer, skal du logge på igen, før du anmoder om en ny token.</span><span class="sxs-lookup"><span data-stu-id="d1f51-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="d1f51-112">Efter 30, 2020, er der ingen ny lejer, der kan bruge politikken for levetiden for konfigurerbare tokens til at konfigurere session og opdatere tokens.</span><span class="sxs-lookup"><span data-stu-id="d1f51-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="d1f51-113">Frarådelsen sker inden for flere måneder efter dette, hvilket betyder, at vi stopper med at overholde eksisterende sessioner og opdaterer tokens.</span><span class="sxs-lookup"><span data-stu-id="d1f51-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="d1f51-114">Du kan stadig konfigurere levetiden for adgangs tokens efter dette frarådes.</span><span class="sxs-lookup"><span data-stu-id="d1f51-114">You can still configure access token lifetimes after the deprecation.</span></span>






