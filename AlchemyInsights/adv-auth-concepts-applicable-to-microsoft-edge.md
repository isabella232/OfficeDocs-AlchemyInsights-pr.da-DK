---
title: Avancerede godkendelses koncepter, der gælder for Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573330"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="8e134-102">Avancerede godkendelses koncepter, der gælder for Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8e134-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="8e134-103">Følgende er de avancerede godkendelses koncepter, der gælder for Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="8e134-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="8e134-104">**Proaktiv godkendelse**</span><span class="sxs-lookup"><span data-stu-id="8e134-104">**Proactive Authentication**</span></span>

<span data-ttu-id="8e134-105">Når du aktiverer [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -politikken, forsøger Microsoft Edge proaktivt at godkende brugere, der er logget på, via Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="8e134-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="8e134-106">Med jævne mellemrum bruges en onlinetjeneste til at kontrollere, om der er et opdateret manifest, der indeholder konfigurationen til proaktiv godkendelse.</span><span class="sxs-lookup"><span data-stu-id="8e134-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="8e134-107">Fordele: proaktiv godkendelse giver mulighed for godkendelse af nøgle tjenester, f. eks den nye faneside i Office.</span><span class="sxs-lookup"><span data-stu-id="8e134-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="8e134-108">Hvis Bing også bruges som søgemaskine, forbedrer proaktiv godkendelse ydeevnen for adresselinjen og hjælper med at oprette søgeresultater, der er tilpasset din virksomheds behov.</span><span class="sxs-lookup"><span data-stu-id="8e134-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="8e134-109">**Windows Hello CredUI til NTLM-godkendelse**</span><span class="sxs-lookup"><span data-stu-id="8e134-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="8e134-110">Hvis enkeltlogon (SSO) ikke er tilgængelig, når et websted forsøger at logge på brugeren via NTLM-eller Negotiate-mekanismen, giver brugeren mulighed for at dele OS-legitimationsoplysninger med webstedet og for at opfylde godkendelses udfordringen ved hjælp af BRUGERGRÆNSEFLADEN i Windows Hello-legitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="8e134-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="8e134-111">Dette tilmeldings forløb vises kun i Windows 10 og kun for brugere, der ikke får SSO under en NTLM-eller en Negotiate-udfordring.</span><span class="sxs-lookup"><span data-stu-id="8e134-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="8e134-112">**Brug gemte adgangskoder til at logge på automatisk**</span><span class="sxs-lookup"><span data-stu-id="8e134-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="8e134-113">Brugere, der gemmer adgangskoder i Microsoft Edge, kan aktivere automatisk logon på websteder, hvor de har gemt dine legitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="8e134-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="8e134-114">Brugere kan slå denne funktion til eller fra i edge://settings/passwords, og du kan konfigurere den i politikker for [adgangskodestyring](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="8e134-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
