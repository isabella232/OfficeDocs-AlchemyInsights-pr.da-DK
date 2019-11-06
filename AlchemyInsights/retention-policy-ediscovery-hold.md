---
title: 2609-tilbageholdelse-eller-eDiscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994054"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="a8b36-102">Kan ikke slette elementer i SharePoint Online eller OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="a8b36-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="a8b36-103">Du eller dine brugere kan muligvis ikke slette elementer i SharePoint Online eller OneDrive for Business, fordi en opbevaringspolitik, en opbevarings etiket eller et eDiscovery-hold anvendes på et SharePoint-websted for OneDrive eller på et bestemt element.</span><span class="sxs-lookup"><span data-stu-id="a8b36-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="a8b36-104">Dette omfatter ikke at kunne slette et dokument, en dokumentversion, en mappe, et dokumentbibliotek, en liste, en app, et websted eller en gruppe af websteder.</span><span class="sxs-lookup"><span data-stu-id="a8b36-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="a8b36-105">Her er nogle eksempler på de fejlmeddelelser, du kan fÃ ¥ modtaget, hvis du forsÃ ̧ger at slette et element, der bevares:</span><span class="sxs-lookup"><span data-stu-id="a8b36-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="a8b36-106">"Dette websted kan ikke slettes, fordi det er medtaget i en e-Discovery-tilbageholdelse eller opbevaringspolitik"</span><span class="sxs-lookup"><span data-stu-id="a8b36-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="a8b36-107">"Dette websted har en overholdelses politik, der er indstillet til at blokere sletningen"</span><span class="sxs-lookup"><span data-stu-id="a8b36-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="a8b36-108">"En overholdelses politik blokerer i øjeblikket for sletningen af webstedet"</span><span class="sxs-lookup"><span data-stu-id="a8b36-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="a8b36-109">"Denne gruppe af websteder kan ikke slettes, fordi den indeholder websteder, der er inkluderet i en hold-eller opbevaringspolitik for eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="a8b36-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="a8b36-110">"Du er nødt til at slette alle emnerne i denne mappe, før du sletter mappen"</span><span class="sxs-lookup"><span data-stu-id="a8b36-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="a8b36-111">"Versioner af dette element kan ikke slettes, fordi det er i hold-eller opbevaringspolitik"</span><span class="sxs-lookup"><span data-stu-id="a8b36-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="a8b36-112">"Elementet kan ikke slettes, mens det er i hold"</span><span class="sxs-lookup"><span data-stu-id="a8b36-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="a8b36-113">"Den etiket, der anvendes på dette element, forhindrer, at den redigeres eller slettes"</span><span class="sxs-lookup"><span data-stu-id="a8b36-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="a8b36-114">"Listen kan ikke slettes, mens den er i hold-eller opbevaringspolitik"</span><span class="sxs-lookup"><span data-stu-id="a8b36-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="a8b36-115">"Listen kan ikke slettes, hvis den er blokeret, eller hvis der er anvendt en opbevaringspolitik på den"</span><span class="sxs-lookup"><span data-stu-id="a8b36-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="a8b36-116">Hvis du vil slette elementer i et af disse scenarier, skal opbevaringspolitikken, opbevarings etiketten eller eDiscovery-hold fjernes (eller et websted skal udelukkes fra en opbevaringspolitik).</span><span class="sxs-lookup"><span data-stu-id="a8b36-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="a8b36-117">Du skal enten deaktivere eller udelukke respektive hold, der forårsager dette problem.</span><span class="sxs-lookup"><span data-stu-id="a8b36-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a8b36-118">Når en opbevaringspolitik eller et hold er fjernet, kan det tage op til 24 timer, indtil ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="a8b36-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="a8b36-119">Du kan finde oplysninger om de forskellige funktioner til fastholdelse og tilbageholdelse, der gælder for SharePoint-websteder og OneDrive-konti, under et af følgende emner.</span><span class="sxs-lookup"><span data-stu-id="a8b36-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="a8b36-120">Oversigt over opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="a8b36-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="a8b36-121">Oversigt over opbevarings etiketter</span><span class="sxs-lookup"><span data-stu-id="a8b36-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="a8b36-122">Administrer ventepositioner i avanceret eDiscovery</span><span class="sxs-lookup"><span data-stu-id="a8b36-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="a8b36-123">eDiscovery holder</span><span class="sxs-lookup"><span data-stu-id="a8b36-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="a8b36-124">Politikker for lukning og sletning af ældre websteder</span><span class="sxs-lookup"><span data-stu-id="a8b36-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
