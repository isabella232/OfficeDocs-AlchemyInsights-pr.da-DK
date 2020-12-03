---
title: Slet lejer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564487"
---
# <a name="delete-tenant"></a><span data-ttu-id="b75e3-102">Slet lejer</span><span class="sxs-lookup"><span data-stu-id="b75e3-102">Delete tenant</span></span>

<span data-ttu-id="b75e3-103">Hvis du vil slette en Azure AD, skal du sikre:</span><span class="sxs-lookup"><span data-stu-id="b75e3-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="b75e3-104">Du er Global administrator på adresselisten.</span><span class="sxs-lookup"><span data-stu-id="b75e3-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="b75e3-105">Du er ikke logget på med en konto, der har standardmappen som f. eks contoso.onmicrosoft.com på den konto, der er logget på, f. eks admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b75e3-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="b75e3-106">Fjern eventuelle aktive programmer i kataloget, før de slettes.</span><span class="sxs-lookup"><span data-stu-id="b75e3-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="b75e3-107">Hvis du vil fjerne aktive programmer, skal du gå til App-registreringer og fjerne eksisterende programmer.</span><span class="sxs-lookup"><span data-stu-id="b75e3-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="b75e3-108">Der er ingen aktive abonnementer til Microsoft online-tjenester, såsom Microsoft Azure, Office 365 eller Azure AD Premium, der er knyttet til kataloget.</span><span class="sxs-lookup"><span data-stu-id="b75e3-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="b75e3-109">Overfør dine abonnementer, eller fremskyndelse af aktive abonnementer via Azure support og fakturering.</span><span class="sxs-lookup"><span data-stu-id="b75e3-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="b75e3-110">Få mere at vide om, hvordan du annullerer Office 365 og Azure-abonnementer.</span><span class="sxs-lookup"><span data-stu-id="b75e3-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="b75e3-111">Du kan finde en vejledning til, hvordan du knytter eller tilføjer et eksisterende abonnement til en lejer, under [tilknytte eller tilføje et Azure-abonnement til din Azure ad-lejer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b75e3-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="b75e3-112">Der er ingen aktiv licens.</span><span class="sxs-lookup"><span data-stu-id="b75e3-112">There are no Active license.</span></span> <span data-ttu-id="b75e3-113">Hvis du vil fjerne licenser, skal du se [Sådan fjerner du abonnementet for at fjerne licensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="b75e3-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="b75e3-114">Der er ingen andre aktive brugere i oversigten ud over selv som den globale administrator, når de forsøger at slette Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b75e3-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="b75e3-115">Fjern eventuelle andre aktive brugere, og afhængigheder på et brugerdefineret domænenavn i lejeren skal også fjernes, f. eks brugere oprettet med admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b75e3-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="b75e3-116">Du kan finde flere oplysninger om, hvordan du gør følgende:</span><span class="sxs-lookup"><span data-stu-id="b75e3-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="b75e3-117">Slet "Azure Active Directory" eller "abonnement", se [Slet Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="b75e3-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="b75e3-118">Hvis du vil fjerne programmer i mappen, skal du se [fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="b75e3-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
