---
title: Avancerede godkendelseskoncepter, der gælder for Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398550"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="2ca47-102">Avancerede godkendelseskoncepter, der gælder for Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2ca47-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="2ca47-103">Følgende er de avancerede godkendelseskoncepter, der gælder for Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="2ca47-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="2ca47-104">**Proactive Authentication**</span><span class="sxs-lookup"><span data-stu-id="2ca47-104">**Proactive Authentication**</span></span>

<span data-ttu-id="2ca47-105">Når du aktiverer [politikken ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) vil Microsoft Edge forsøge proaktivt at godkende brugere, der er logget på via Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="2ca47-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="2ca47-106">Med jævne mellemrum vil den bruge en onlinetjeneste til at kontrollere, om der er et opdateret manifest, der indeholder den konfiguration, der styrer Proaktiv godkendelse.</span><span class="sxs-lookup"><span data-stu-id="2ca47-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="2ca47-107">Fordele: Proaktiv godkendelse giver godkendelse adgang til vigtige tjenester, f.eks. siden ny fane i Office.</span><span class="sxs-lookup"><span data-stu-id="2ca47-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="2ca47-108">Hvis Bing bruges som søgemaskine, forbedrer Proaktiv godkendelse også ydeevnen af adresselinjen og hjælper med at generere søgeresultater, der er tilpasset behovene i din virksomhed.</span><span class="sxs-lookup"><span data-stu-id="2ca47-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="2ca47-109">**Windows Hello CredUI til NTLM-godkendelse**</span><span class="sxs-lookup"><span data-stu-id="2ca47-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="2ca47-110">Hvis enkelt-logon (SSO) ikke er tilgængelig, når et websted forsøger at logge på brugeren via mekanismen NTLM eller Forhandl, giver denne funktion brugeren mulighed for at dele os-legitimationsoplysningerne med webstedet og opfylde godkendelsesudfordringen ved hjælp af Windows Hello Cred-brugergrænsefladen.</span><span class="sxs-lookup"><span data-stu-id="2ca47-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="2ca47-111">Dette logonflow vises kun i Windows 10 og kun for brugere, der ikke får SSO under en NTLM- eller en forhandl-udfordring.</span><span class="sxs-lookup"><span data-stu-id="2ca47-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="2ca47-112">**Brug gemte adgangskoder til at logge på automatisk**</span><span class="sxs-lookup"><span data-stu-id="2ca47-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="2ca47-113">Brugere, der gemmer adgangskoder i Microsoft Edge, kan aktivere automatisk logon på websteder, hvor de har gemt legitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="2ca47-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="2ca47-114">Brugere kan slå denne funktion til eller fra i edge://settings/passwords, og du kan konfigurere den i [politikkerne for adgangskodestyring.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="2ca47-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
