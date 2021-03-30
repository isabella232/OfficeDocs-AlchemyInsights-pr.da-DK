---
title: Single-Sign aktiveret til Enheder, der er forbundet med Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404589"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="fecb1-102">Enkelt-logon til Azure Active Directory-enheder, der er forbundet</span><span class="sxs-lookup"><span data-stu-id="fecb1-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="fecb1-103">Hvis du har et lokalt Active Directory-miljø (AD), og du vil slutte dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse.</span><span class="sxs-lookup"><span data-stu-id="fecb1-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="fecb1-104">[Sådan gør du: Planlæg din hybride](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) implementering af Azure Active Directory-joinforbindelse giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.</span><span class="sxs-lookup"><span data-stu-id="fecb1-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="fecb1-105">Konfigurere enheder, der er forbundet til Azure AD, til lokale Single-Sign til ved hjælp af Windows Hello til virksomheder</span><span class="sxs-lookup"><span data-stu-id="fecb1-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="fecb1-106">**Problemer med primær opdateringstoken (PRT)** Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10-, Windows Server 2016- og nyere versioner, iOS- og Android-enheder.</span><span class="sxs-lookup"><span data-stu-id="fecb1-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="fecb1-107">Det er en JSON Web Token (JWT), der er særligt udstedt til Microsofts token-formidlere af første part for at aktivere enkelt-logon (SSO) på tværs af de programmer, der bruges på disse enheder.</span><span class="sxs-lookup"><span data-stu-id="fecb1-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="fecb1-108">[I Hvad er en primær opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), angiver vi oplysninger om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10-enheder.</span><span class="sxs-lookup"><span data-stu-id="fecb1-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="fecb1-109">**WamDefaultSet: YES og AzureADPrt: YES** Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når der logges på enheden.</span><span class="sxs-lookup"><span data-stu-id="fecb1-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="fecb1-110">Hvis værdierne er NEJ, **kan** det være forfaldent:</span><span class="sxs-lookup"><span data-stu-id="fecb1-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="fecb1-111">Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (kontrollér KeySignTest, mens den kører med administrator administrator).</span><span class="sxs-lookup"><span data-stu-id="fecb1-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="fecb1-112">Alternativt logon-id</span><span class="sxs-lookup"><span data-stu-id="fecb1-112">Alternate Login ID</span></span>
- <span data-ttu-id="fecb1-113">HTTP-proxy blev ikke fundet</span><span class="sxs-lookup"><span data-stu-id="fecb1-113">HTTP Proxy not found</span></span>

<span data-ttu-id="fecb1-114">Fejlfinding af enheder ved hjælp af kommandoen dsregcmd – [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="fecb1-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
