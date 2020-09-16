---
title: Forsinkelser i modtagelse af SharePoint-og OneDrive-beskeder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727237"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="c96b7-102">Forsinkelser i modtagelse af SharePoint-og OneDrive-beskeder</span><span class="sxs-lookup"><span data-stu-id="c96b7-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="c96b7-103">Kontrollér først mappen uønsket mail eller spam i din mail.</span><span class="sxs-lookup"><span data-stu-id="c96b7-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="c96b7-104">Hvis **alle beskeder fra flere filer eller biblioteker forsinkes**, skal du gå til [tjeneste tilstands dashboardet](https://portal.office.com/adminportal/home?ref=/servicehealth) for at kontrollere, om der er nogen rådgivere/Incidents, der kan forekomme i SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="c96b7-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="c96b7-105">Problemet kan skyldes SharePoint-beskedfunktionen eller-forsinkelser i mails via Exchange.</span><span class="sxs-lookup"><span data-stu-id="c96b7-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="c96b7-106">Bemærk også, om der leveres andre mails – hvis ikke, er problemet sandsynligt med Exchange-forsinkelser.</span><span class="sxs-lookup"><span data-stu-id="c96b7-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="c96b7-107">Hvis **en individuel besked fra en bestemt fil eller et bestemt bibliotek ikke er leveret**, skal du forsøge at slette og gendanne den.</span><span class="sxs-lookup"><span data-stu-id="c96b7-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="c96b7-108">Se [Administrer, få vist eller Slet SharePoint-beskeder](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for at genoprette beskeden.</span><span class="sxs-lookup"><span data-stu-id="c96b7-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="c96b7-109">Der kan ikke sendes beskeder til en distributionsgruppe.</span><span class="sxs-lookup"><span data-stu-id="c96b7-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="c96b7-110">Kun sikkerheds-og O365-grupper understøttes.</span><span class="sxs-lookup"><span data-stu-id="c96b7-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="c96b7-111">Du kan ikke tilpasse mailskabeloner til påmindelser.</span><span class="sxs-lookup"><span data-stu-id="c96b7-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="c96b7-112">Du skal bruge Microsoft flow-eller SharePoint Designer-arbejdsproces for at opnå dem.</span><span class="sxs-lookup"><span data-stu-id="c96b7-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
