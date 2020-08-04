---
title: Problemer med at bruge Intune-administrationskonsollen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554882"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="265e4-102">Problemer med at bruge Intune-administrationskonsollen</span><span class="sxs-lookup"><span data-stu-id="265e4-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="265e4-103">**"Adgang nægtet", når du navigerer i Intune-administrationsportalen.**</span><span class="sxs-lookup"><span data-stu-id="265e4-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="265e4-104">Hvis du er medlem af en brugerdefineret Intune-rolle, skal du sikre dig, at der er tildelt en INtune- eller Enterprise Mobility Suite-licens (EMS) til din konto.</span><span class="sxs-lookup"><span data-stu-id="265e4-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="265e4-105">Hvis du bruger Konfigurationsstyring til at administrere enheder, skal du kontrollere, at du ikke er en del af Intune-brugersamlingen for Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="265e4-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="265e4-106">Kontroller, at du har fået tildelt de relevante rollebaserede rbac-tilladelser (Role-based Administration Control) i bladet Intune-roller.</span><span class="sxs-lookup"><span data-stu-id="265e4-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="265e4-107">Kontroller, at den anvendte gruppe ikke er en distributionsliste.</span><span class="sxs-lookup"><span data-stu-id="265e4-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="265e4-108">Intune på Azure-portalen understøtter kun brugerkonti, der tilhører Azure Active Directory-sikkerhedsgrupper.</span><span class="sxs-lookup"><span data-stu-id="265e4-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="265e4-109">Gennemse dine grupper i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="265e4-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="265e4-110">**Brugeren har for mange tilladelser til tildelt intune-rollen**</span><span class="sxs-lookup"><span data-stu-id="265e4-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="265e4-111">Råd til brugeren om at gå **til Intune**  >  **Intune-roller Mine**tilladelser  >  **My permissions**  >  **Eksporter for** at gennemse tildelte tilladelser.</span><span class="sxs-lookup"><span data-stu-id="265e4-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="265e4-112">**Jeg har føjet en områdegruppe til en rolle, men brugere i den rolle kan stadig se andre brugere eller enheder.**</span><span class="sxs-lookup"><span data-stu-id="265e4-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="265e4-113">Områdegrupper bortfiltrer ikke brugere eller enheder.</span><span class="sxs-lookup"><span data-stu-id="265e4-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="265e4-114">Områdegrupper:</span><span class="sxs-lookup"><span data-stu-id="265e4-114">Scope groups:</span></span>

- <span data-ttu-id="265e4-115">Begræns, hvem brugere kan tildele politikker eller programmer til.</span><span class="sxs-lookup"><span data-stu-id="265e4-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="265e4-116">Tillad kun bestemte brugere at køre fjernopgaver på enheder.</span><span class="sxs-lookup"><span data-stu-id="265e4-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="265e4-117">Yderligere oplysninger om områdegrupper finder du [i Role-based access control (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="265e4-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="265e4-118">**Jeg har føjet en bruger til en Intune-rolle, men de har stadig fuld adgang til Intune-administrationskonsollen.**</span><span class="sxs-lookup"><span data-stu-id="265e4-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="265e4-119">Gå til Intune > **Brugere** i Azure-portalen, og kontroller, at brugeren ikke er tildelt nogen af følgende roller på Azure-portalen:</span><span class="sxs-lookup"><span data-stu-id="265e4-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="265e4-120">Global administrator</span><span class="sxs-lookup"><span data-stu-id="265e4-120">Global administrator</span></span>
- <span data-ttu-id="265e4-121">Intune-tjenesteadministrator</span><span class="sxs-lookup"><span data-stu-id="265e4-121">Intune service administrator</span></span>
- <span data-ttu-id="265e4-122">SharePoint-administrator</span><span class="sxs-lookup"><span data-stu-id="265e4-122">SharePoint administrator</span></span>

<span data-ttu-id="265e4-123">Yderligere oplysninger finder du [i Role-based access control (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="265e4-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="265e4-124">**Problemer med adgang**</span><span class="sxs-lookup"><span data-stu-id="265e4-124">**Access Issues**</span></span>

<span data-ttu-id="265e4-125">Du kan finde flere oplysninger [under Du kan ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="265e4-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>