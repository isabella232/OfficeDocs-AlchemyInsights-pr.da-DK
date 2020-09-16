---
title: Problemer med at bruge Intune-administrationskonsollen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728281"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="1bc58-102">Problemer med at bruge Intune-administrationskonsollen</span><span class="sxs-lookup"><span data-stu-id="1bc58-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="1bc58-103">**"Adgang nægtet", når du navigerer til Intune-administrations portalen.**</span><span class="sxs-lookup"><span data-stu-id="1bc58-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="1bc58-104">Hvis du er medlem af en brugerdefineret Intune-rolle, skal du sikre dig, at en Intune-eller Enterprise Mobility Suite-licens (EMS) er tildelt til din konto.</span><span class="sxs-lookup"><span data-stu-id="1bc58-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="1bc58-105">Hvis du bruger Konfigurationsstyring til at administrere enheder, skal du kontrollere, at du ikke er en del af Intune-bruger samlingen for Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="1bc58-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="1bc58-106">Kontrollér, at du er blevet tildelt den relevante rollebaserede administrations kontrol (RBAC)-tilladelser i blade til Intune-roller.</span><span class="sxs-lookup"><span data-stu-id="1bc58-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="1bc58-107">Kontrollér, at den anvendte gruppe ikke er en distributionsliste.</span><span class="sxs-lookup"><span data-stu-id="1bc58-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="1bc58-108">Intune i Azure-portalen understøtter kun brugerkonti, der hører til Azure Active Directory-sikkerhedsgrupper.</span><span class="sxs-lookup"><span data-stu-id="1bc58-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="1bc58-109">Gennemse dine grupper i Azure-portalen > **Intune**  >  -**grupper**eller i Azure-portalen > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="1bc58-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="1bc58-110">**Brugeren har for mange tilladelser til den tildelte Intune-rolle**</span><span class="sxs-lookup"><span data-stu-id="1bc58-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="1bc58-111">Adviser brugeren om at gå til **Intune**  >  **Intune-roller**  >  **mine tilladelser**  >  **eksport** for at gennemse de tilladelser, der er tildelt.</span><span class="sxs-lookup"><span data-stu-id="1bc58-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="1bc58-112">**Jeg har føjet en områdegruppe til en rolle, men brugere i den pågældende rolle stadig kan se andre brugere eller enheder.**</span><span class="sxs-lookup"><span data-stu-id="1bc58-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="1bc58-113">Områdegrupper filtrerer ikke brugere eller enheder.</span><span class="sxs-lookup"><span data-stu-id="1bc58-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="1bc58-114">Områdegrupper:</span><span class="sxs-lookup"><span data-stu-id="1bc58-114">Scope groups:</span></span>

- <span data-ttu-id="1bc58-115">Begræns, hvem brugere kan tildele politikker eller programmer til.</span><span class="sxs-lookup"><span data-stu-id="1bc58-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="1bc58-116">Tillad kun bestemte brugere at køre eksterne opgaver på enheder.</span><span class="sxs-lookup"><span data-stu-id="1bc58-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="1bc58-117">Du kan finde flere oplysninger om områdegrupper under  [rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="1bc58-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="1bc58-118">**Jeg har føjet en bruger til en Intune-rolle, men de har stadig fuld adgang til Intune-administrationskonsollen.**</span><span class="sxs-lookup"><span data-stu-id="1bc58-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="1bc58-119">Naviger til Intune > **brugere** i Azure-portalen, og kontrollér, at brugeren ikke er tildelt en af følgende roller i Azure-portalen:</span><span class="sxs-lookup"><span data-stu-id="1bc58-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="1bc58-120">Global administrator</span><span class="sxs-lookup"><span data-stu-id="1bc58-120">Global administrator</span></span>
- <span data-ttu-id="1bc58-121">Intune-tjenesteadministrator</span><span class="sxs-lookup"><span data-stu-id="1bc58-121">Intune service administrator</span></span>
- <span data-ttu-id="1bc58-122">SharePoint-administrator</span><span class="sxs-lookup"><span data-stu-id="1bc58-122">SharePoint administrator</span></span>

<span data-ttu-id="1bc58-123">Du kan finde flere oplysninger under [rollebaseret adgangskontrol (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="1bc58-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="1bc58-124">**Adgangsproblemer**</span><span class="sxs-lookup"><span data-stu-id="1bc58-124">**Access Issues**</span></span>

<span data-ttu-id="1bc58-125">Du kan finde flere oplysninger i [kan du ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="1bc58-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>