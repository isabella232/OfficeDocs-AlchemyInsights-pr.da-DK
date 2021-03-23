---
title: Problemer med brugeradministration
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035529"
---
# <a name="user-management-issues"></a><span data-ttu-id="2bf2f-102">Problemer med brugeradministration</span><span class="sxs-lookup"><span data-stu-id="2bf2f-102">User management issues</span></span>

<span data-ttu-id="2bf2f-103">**Hvad sker der med aktuelle tildelte brugere til programmet, hvis jeg deaktiverer egenskaben "Brugertildeling påkrævet" (angiv denne egenskab til Nej)?**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="2bf2f-104">Deaktivering **af brugertildeling påkrævet** påvirker IKKE de aktuelt tildelte brugere.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="2bf2f-105">Deaktivering af denne egenskab tillader kun alle brugere at få adgang til programmet.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="2bf2f-106">Alle de viste brugere og de brugere, der er tildelt grupper i programmet, vil stadig være gyldige.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="2bf2f-107">Hvis du vil begrænse din app til bestemte brugere, skal du se : Begræns Azure AD-appen til en række brugere [– Microsoft-identitetsplatformen | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="2bf2f-108">Hvis du vil tildele brugere og grupper til virksomhedsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjælp af PowerShell, skal du se Administrer brugertildeling for en app i [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="2bf2f-109">Hvis du vil uddelegere tilladelser til oprettelse og administration af programmer, skal du se Stedfortrædertilladelser til [programadministration – Azure AD-| Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="2bf2f-110">**Skjul bestemte virksomhedsapps for brugere** – Brug følgende trin til at skjule alle Microsoft 365-apps **fra panelet MyApps.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="2bf2f-111">Appsene vil stadig være synlige på Office 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="2bf2f-112">Log på Azure-portalen som global administrator for dit katalog.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="2bf2f-113">Vælg **Azure Active Directory.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="2bf2f-114">Vælg **Brugere.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="2bf2f-115">Vælg **Brugerindstillinger.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="2bf2f-116">Under **Virksomhedsprogrammer skal** du klikke **på Administrer, hvordan slutbrugere starter og får vist deres programmer.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="2bf2f-117">For **brugere kan kun se Office 365-apps i Office 365-portalen** skal du klikke på **Ja.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="2bf2f-118">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="2bf2f-119">Få mere at vide under [Skjul et Enterprise-program fra brugerens oplevelse i Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="2bf2f-120">Hvis du tilbyder en SaaS-app (Software as a Service) til mange organisationer, kan du konfigurere din app til at acceptere logons fra alle Azure Active Directory-lejere (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2bf2f-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="2bf2f-121">Denne konfiguration kaldes "gør dit program til flere lejere".</span><span class="sxs-lookup"><span data-stu-id="2bf2f-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="2bf2f-122">Brugere i alle Azure AD-lejere vil kunne logge på din app, når de har accepteret at bruge deres konto med din app.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="2bf2f-123">Få mere at vide under [Opbyg apps, der logger på Azure AD-brugere – Microsoft-identitetsplatformen | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="2bf2f-124">**Hvordan kan en slutbruger få adgang til programmet, når han/hun er tildelt til programmet?**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="2bf2f-125">Hver app i Enterprise-program bladet har et link, som slutbrugere kan få adgang til.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="2bf2f-126">Brugere kan også få adgang til appen **via Myapps-portalen** på en nem måde.</span><span class="sxs-lookup"><span data-stu-id="2bf2f-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="2bf2f-127">**Vil du gerne vide, hvilke programmer og programtyper brugerne bruger?**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="2bf2f-128">Du kan hente logonrapporter for de seneste 30 dage fra portal.azure.com > Azure Active Directory> **Signins> overførselsrapporter.**</span><span class="sxs-lookup"><span data-stu-id="2bf2f-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="2bf2f-129">Få mere at vide [om, hvordan du giver administratorsamtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for hele lejeren og [konfigurerer slutbrugernes samtykke til programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="2bf2f-130">Forstå, [hvordan samtykke fungerer,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [og Administrer samtykke til programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)</span><span class="sxs-lookup"><span data-stu-id="2bf2f-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


