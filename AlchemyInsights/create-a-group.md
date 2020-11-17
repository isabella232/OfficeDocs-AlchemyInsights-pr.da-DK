---
title: Opret en gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088688"
---
# <a name="create-a-group"></a><span data-ttu-id="13017-102">Opret en gruppe</span><span class="sxs-lookup"><span data-stu-id="13017-102">Create a group</span></span>

<span data-ttu-id="13017-103">I dette emne beskrives gruppe oprettelse.</span><span class="sxs-lookup"><span data-stu-id="13017-103">This topic describes group creation.</span></span>

<span data-ttu-id="13017-104">**Tilladelse til at oprette en gruppe**</span><span class="sxs-lookup"><span data-stu-id="13017-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="13017-105">Sørg for, at du har tilladelse til at oprette en ny gruppe.</span><span class="sxs-lookup"><span data-stu-id="13017-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="13017-106">Globale administratorer kan deaktivere gruppe oprettelse i Azure-portalen eller Access-panelet.</span><span class="sxs-lookup"><span data-stu-id="13017-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="13017-107">Du skal muligvis have en administrator for at oprette den nye gruppe for dig, eller for at give dig de relevante tilladelser.</span><span class="sxs-lookup"><span data-stu-id="13017-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="13017-108">**Administrer tilladelser til gruppe oprettelse**</span><span class="sxs-lookup"><span data-stu-id="13017-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="13017-109">Globale administratorer kan administrere tilladelser til gruppe oprettelse (for sikkerhedsrelaterede årsager) eller Office 365-grupper, der er oprettet i Azure-portalen eller Access-panelet, ved at vælge "brugerne kan oprette sikkerhedsgrupper i Azure-portaler" eller "brugerne kan oprette Office 365-grupper i Azure-portaler" i **alle grupperne**  >  **Generelt (indstillinger)**.</span><span class="sxs-lookup"><span data-stu-id="13017-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="13017-110">Du kan også begrænse oprettelse af gruppe for at vælge en gruppe af brugere, hvis du har en Azure Active Directory P1 Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="13017-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="13017-111">**Deaktivering af velkomstmeddelelse for nye Office 365-gruppemedlemmer**</span><span class="sxs-lookup"><span data-stu-id="13017-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="13017-112">Den velkomstmeddelelse, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at angive **UnifiedGroupWelcomeMessageEnabled** til falsk i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="13017-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="13017-113">Få mere at vide om denne indstilling [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="13017-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

