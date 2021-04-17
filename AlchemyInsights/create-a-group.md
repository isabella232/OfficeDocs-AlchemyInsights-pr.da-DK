---
title: Opret en gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816342"
---
# <a name="create-a-group"></a><span data-ttu-id="9b2f3-102">Opret en gruppe</span><span class="sxs-lookup"><span data-stu-id="9b2f3-102">Create a group</span></span>

<span data-ttu-id="9b2f3-103">I dette emne beskrives oprettelse af grupper.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-103">This topic describes group creation.</span></span>

<span data-ttu-id="9b2f3-104">**Tilladelse til at oprette en gruppe**</span><span class="sxs-lookup"><span data-stu-id="9b2f3-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="9b2f3-105">Sørg for, at du er godkendt til at oprette en ny gruppe.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="9b2f3-106">Globale administratorer kan deaktivere oprettelse af grupper i Azure-portalen eller adgangspanelet.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="9b2f3-107">Du skal muligvis have en administrator for at oprette den nye gruppe for dig eller for at give dig de relevante tilladelser.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="9b2f3-108">**Administrere tilladelser til oprettelse af grupper**</span><span class="sxs-lookup"><span data-stu-id="9b2f3-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="9b2f3-109">Globale administratorer kan administrere tilladelser til oprettelse af grupper (af sikkerhedsrelaterede årsager) eller Office 365-grupper, der er oprettet i Azure-portalen eller adgangspanelet, ved at vælge indstillingerne "Brugere kan oprette sikkerhedsgrupper i Azure-portaler" eller "Brugere kan oprette Office 365-grupper i Azure-portaler" i Alle grupper Generelt  >  **(Indstillinger).**</span><span class="sxs-lookup"><span data-stu-id="9b2f3-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="9b2f3-110">Du kan også begrænse oprettelse af grupper for at vælge en gruppe af brugere, hvis du har en Azure Active Directory P1 Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="9b2f3-111">**Deaktivere velkomstmeddelelse for nye Office 365-gruppemedlemmer**</span><span class="sxs-lookup"><span data-stu-id="9b2f3-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="9b2f3-112">Velkomstmeddelelsen, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at angive **UnifiedGroupWelcomeMessageEnabled** til False i Powershell.</span><span class="sxs-lookup"><span data-stu-id="9b2f3-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="9b2f3-113">Få mere at vide om denne [indstilling her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9b2f3-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

