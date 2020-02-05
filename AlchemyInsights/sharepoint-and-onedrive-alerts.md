---
title: Forsinkelser i modtagelsen af Beskeder i SharePoint og OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771209"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="98f53-102">Forsinkelser i modtagelsen af Beskeder i SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="98f53-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="98f53-103">Tjek først mappen Uønsket eller Spam i din e-mail.</span><span class="sxs-lookup"><span data-stu-id="98f53-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="98f53-104">Hvis **alle beskeder fra flere filer eller biblioteker er forsinkede,** skal du gå til [dashboardet Tjenestetilstand](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) for at kontrollere, om der kan opstå meddelelser/hændelser med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="98f53-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="98f53-105">Problemet kan være med SharePoint-beskedfunktionen eller forsinkelser i mails via Exchange.</span><span class="sxs-lookup"><span data-stu-id="98f53-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="98f53-106">Bemærk også, om andre e-mails leveres – hvis ikke, er problemet sandsynligvis med Exchange-forsinkelser.</span><span class="sxs-lookup"><span data-stu-id="98f53-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="98f53-107">Hvis **en individuel besked fra en bestemt fil eller et bestemt bibliotek ikke leveres**, skal du forsøge at slette og genoprette den.</span><span class="sxs-lookup"><span data-stu-id="98f53-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="98f53-108">Se [Administrere, få vist eller slette SharePoint-beskeder](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) for at genoprette beskeden.</span><span class="sxs-lookup"><span data-stu-id="98f53-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="98f53-109">Påmindelser kan ikke sendes til en distributionsgruppe.</span><span class="sxs-lookup"><span data-stu-id="98f53-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="98f53-110">Kun grupper sikkerhed og O365 understøttes.</span><span class="sxs-lookup"><span data-stu-id="98f53-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="98f53-111">Du kan ikke tilpasse beskedmailskabeloner.</span><span class="sxs-lookup"><span data-stu-id="98f53-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="98f53-112">Du skal bruge Microsoft Flow- eller SharePoint Designer Workflow for at opnå disse.</span><span class="sxs-lookup"><span data-stu-id="98f53-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
