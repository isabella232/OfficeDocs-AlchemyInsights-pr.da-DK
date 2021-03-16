---
title: Fejlfinding af Seamless Single Sign-on (SSO) i det lokale miljø
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816129"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="44465-102">Fejlfinding af Seamless Single Sign-on (SSO) i det lokale miljø</span><span class="sxs-lookup"><span data-stu-id="44465-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="44465-103">For at løse problemer med enkelt logon (Seamless Single Sign-on– SSO) skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="44465-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="44465-104">**Hvordan kan jeg rulle over Kerberos- dekrypteringsnøglen til AZUREADSSO-computerkontoen?**</span><span class="sxs-lookup"><span data-stu-id="44465-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="44465-105">Vi anbefaler, at du ruller over Kerberos-dekrypteringsnøglen mindst hver 30. dag.</span><span class="sxs-lookup"><span data-stu-id="44465-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="44465-106">Hvis du vil gøre dette manuelt, skal [du se, hvordan du kan rulle over Kerberos-dekrypteringsnøgler.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="44465-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="44465-107">**Konfigurer problemfri SSO**</span><span class="sxs-lookup"><span data-stu-id="44465-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="44465-108">For at installere Seamless SSO skal du følge trinnene [i Azure Active Directory Seamless Single Sign-On: Hurtigstarter.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="44465-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="44465-109">**Rådgivning**</span><span class="sxs-lookup"><span data-stu-id="44465-109">**Advisory**</span></span>

- <span data-ttu-id="44465-110">[Azure Active Directory Seamless Single Sign-On:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) Ofte stillede spørgsmål – I denne artikel ser vi på ofte stillede spørgsmål om Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="44465-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="44465-111">Fortsæt med at søge efter nyt indhold.</span><span class="sxs-lookup"><span data-stu-id="44465-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="44465-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Denne artikel indeholder oplysninger om, hvordan du anmoder om funktioner eller stiller tekniske spørgsmål om Seamless SSO.</span><span class="sxs-lookup"><span data-stu-id="44465-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="44465-113">**Fejlfinding**</span><span class="sxs-lookup"><span data-stu-id="44465-113">**Troubleshoot**</span></span>

<span data-ttu-id="44465-114">[Fejlfinding af Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) – Denne artikel hjælper dig med at finde fejlfindingsoplysninger om almindelige problemer med Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="44465-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







