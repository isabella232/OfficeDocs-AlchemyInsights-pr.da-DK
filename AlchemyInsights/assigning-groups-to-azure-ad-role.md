---
title: Tildele grupper til Azure AD-rolle
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884911"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="637ca-102">Tildele grupper til Azure AD-rolle</span><span class="sxs-lookup"><span data-stu-id="637ca-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="637ca-103">Hvis du vil tildele en Azure AD-gruppe med kilde til myndighed i Azure AD til en Azure AD-rolle, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="637ca-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="637ca-104">Opret en ny gruppe – for at oprette en ny gruppe:</span><span class="sxs-lookup"><span data-stu-id="637ca-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="637ca-105">a.</span><span class="sxs-lookup"><span data-stu-id="637ca-105">a.</span></span> <span data-ttu-id="637ca-106">Log på Azure AD administration med **privilegeret rolleadministrator** eller **globale administrator** tilladelser.</span><span class="sxs-lookup"><span data-stu-id="637ca-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="637ca-107">b.</span><span class="sxs-lookup"><span data-stu-id="637ca-107">b.</span></span> <span data-ttu-id="637ca-108">Vælg **Azure Active Directory-> grupper > alle grupper > ny gruppe**.</span><span class="sxs-lookup"><span data-stu-id="637ca-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="637ca-109">c.</span><span class="sxs-lookup"><span data-stu-id="637ca-109">c.</span></span> <span data-ttu-id="637ca-110">Opret gruppen.</span><span class="sxs-lookup"><span data-stu-id="637ca-110">Create the group.</span></span>

2. <span data-ttu-id="637ca-111">Tildel gruppen rollen enten undergruppe oprettelse, eller efter at gruppen er oprettet.</span><span class="sxs-lookup"><span data-stu-id="637ca-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="637ca-112">a.</span><span class="sxs-lookup"><span data-stu-id="637ca-112">a.</span></span> <span data-ttu-id="637ca-113">Hvis du vil tildele en rolle til gruppen på tidspunktet for gruppe oprettelsen, kan du skifte til til/fra- **roller i Azure ad, tildeles gruppen** og oprette gruppen.</span><span class="sxs-lookup"><span data-stu-id="637ca-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="637ca-114">b.</span><span class="sxs-lookup"><span data-stu-id="637ca-114">b.</span></span> <span data-ttu-id="637ca-115">Hvis du vil tildele en rolle til gruppen, efter den er blevet oprettet, skal du gå til fanen **tildelte roller** for den netop oprettede gruppe og tildele rollen til gruppen.</span><span class="sxs-lookup"><span data-stu-id="637ca-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="637ca-116">**Administrere medlemskab af en gruppe, der er tildelt til Azure AD-rolle**</span><span class="sxs-lookup"><span data-stu-id="637ca-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="637ca-117">For at undgå udvidelse af rettigheder kan det være, at administratorerne og globale administratorer som standard kun kan ændre medlemskabet af en gruppe, der er tildelt en rolle.</span><span class="sxs-lookup"><span data-stu-id="637ca-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="637ca-118">De kan dog vælge at tildele en ejer af en sådan gruppe og uddelegere denne opgave.</span><span class="sxs-lookup"><span data-stu-id="637ca-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="637ca-119">Hvis du vil have mere at vide om at tildele Cloud-grupper til Azure AD-roller, skal du se [tildele en ad-roller til Cloud-gruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="637ca-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="637ca-120">Du kan finde flere oplysninger om fejlfinding af roller, der er tildelt Cloud-grupper, under [fejlfinding af roller, der er tildelt Cloud-grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="637ca-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





