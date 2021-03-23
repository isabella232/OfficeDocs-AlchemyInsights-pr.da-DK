---
title: Fejlfinding af enkelt-logon til Azure AD-enheder, der er forbundet
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035465"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="185f0-102">Fejlfinding af enkelt-logon til Azure AD-enheder, der er forbundet</span><span class="sxs-lookup"><span data-stu-id="185f0-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="185f0-103">Hvis du har et lokalt Active Directory-miljø (AD), og du vil slutte dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse.</span><span class="sxs-lookup"><span data-stu-id="185f0-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="185f0-104">[Sådan gør du: Planlæg din hybride](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) implementering af Azure Active Directory-joinforbindelse giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.</span><span class="sxs-lookup"><span data-stu-id="185f0-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="185f0-105">Du kan finde flere oplysninger i Konfigurere enheder, der er forbundet til Azure AD, til [lokale Single-Sign Til ved hjælp af Windows Hello til virksomheder.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="185f0-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="185f0-106">**Problemer med primær opdateringstoken (PRT)**</span><span class="sxs-lookup"><span data-stu-id="185f0-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="185f0-107">Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10-, Windows Server 2016- og nyere versioner, iOS- og Android-enheder.</span><span class="sxs-lookup"><span data-stu-id="185f0-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="185f0-108">Det er en JSON Web Token (JWT), der er særligt udstedt til Microsofts token-formidlere af første part for at aktivere enkelt-logon (SSO) på tværs af de programmer, der bruges på disse enheder.</span><span class="sxs-lookup"><span data-stu-id="185f0-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="185f0-109">Hvis du vil have mere at vide om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10-enheder, skal du se [Hvad er et primært opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="185f0-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="185f0-110">**WamDefaultSet: YES og AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="185f0-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="185f0-111">Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når han/hun logger på enheden.</span><span class="sxs-lookup"><span data-stu-id="185f0-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="185f0-112">Hvis værdierne er **NEJ,** kan det skyldes:</span><span class="sxs-lookup"><span data-stu-id="185f0-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="185f0-113">Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (markér KeySignTest, mens den kører med administrator)</span><span class="sxs-lookup"><span data-stu-id="185f0-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="185f0-114">Alternativt logon-id</span><span class="sxs-lookup"><span data-stu-id="185f0-114">Alternate Login ID</span></span>
- <span data-ttu-id="185f0-115">HTTP-proxy blev ikke fundet</span><span class="sxs-lookup"><span data-stu-id="185f0-115">HTTP Proxy not found</span></span>

<span data-ttu-id="185f0-116">Hvis du vil foretage fejlfinding af enheder, der bruger kommandoen dsregcmd, skal du se [SSO-tilstand.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="185f0-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
