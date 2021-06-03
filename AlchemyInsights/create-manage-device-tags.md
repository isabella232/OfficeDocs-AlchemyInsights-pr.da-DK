---
title: Opret og administrer enhedsmærker eller grupper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731448"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="63b49-102">Opret og administrer enhedsmærker eller grupper</span><span class="sxs-lookup"><span data-stu-id="63b49-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="63b49-103">Tilføj mærker på enheder for at oprette en logisk gruppetilhørsforhold.</span><span class="sxs-lookup"><span data-stu-id="63b49-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="63b49-104">Enhedsmærker understøtter korrekt tilknytning af netværket, så du kan vedhæfte forskellige mærker for at registrere kontekst og aktivere dynamisk oprettelse af lister som en del af en hændelse.</span><span class="sxs-lookup"><span data-stu-id="63b49-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="63b49-105">Mærker kan bruges som et filter i listevisningen Enheder eller til at gruppere enheder.</span><span class="sxs-lookup"><span data-stu-id="63b49-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="63b49-106">Du kan finde flere oplysninger om gruppering af enheder under [Opret og administrer enhedsmærker](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="63b49-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="63b49-107">Du kan tilføje mærker på enheder ved at:</span><span class="sxs-lookup"><span data-stu-id="63b49-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="63b49-108">Brug af portalen</span><span class="sxs-lookup"><span data-stu-id="63b49-108">Using the portal</span></span>

- <span data-ttu-id="63b49-109">Indstilling af en registreringsdatabasenøgleværdi</span><span class="sxs-lookup"><span data-stu-id="63b49-109">Setting a registry key value</span></span>
 
<span data-ttu-id="63b49-110">**Bemærk!** Der kan være ventetid mellem det tidspunkt, hvor et mærke føjes til en enhed, og dens tilgængelighed på listen over enheder og på siden enhed.</span><span class="sxs-lookup"><span data-stu-id="63b49-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="63b49-111">Hvis du vil tilføje enhedsmærker ved hjælp af API, skal [du se Tilføj eller fjern enhedsmærkers API.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="63b49-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="63b49-112">Tilføje og administrere enhedsmærker ved hjælp af portalen</span><span class="sxs-lookup"><span data-stu-id="63b49-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="63b49-113">Vælg den enhed, du vil administrere mærker for.</span><span class="sxs-lookup"><span data-stu-id="63b49-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="63b49-114">Du kan vælge eller søge efter en enhed fra en af følgende visninger:</span><span class="sxs-lookup"><span data-stu-id="63b49-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="63b49-115">**Dashboard for sikkerhedshandlinger** Vælg navnet på enheden i sektionen Bedste enheder med aktive beskeder.</span><span class="sxs-lookup"><span data-stu-id="63b49-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="63b49-116">**Kø til beskeder** – Vælg enhedsnavnet ud for enhedsikonet i køen med vigtige beskeder.</span><span class="sxs-lookup"><span data-stu-id="63b49-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="63b49-117">**Listen Enheder** – Vælg navnet på enheden på listen over enheder.</span><span class="sxs-lookup"><span data-stu-id="63b49-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="63b49-118">**Søgefelt** – Vælg Enhed i rullemenuen, og angiv enhedsnavnet.</span><span class="sxs-lookup"><span data-stu-id="63b49-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="63b49-119">Du kan også få adgang til påmindelsessiden gennem fil- og IP-visningerne.</span><span class="sxs-lookup"><span data-stu-id="63b49-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="63b49-120">Vælg **Administrer mærker** fra rækken af Svarhandlinger.</span><span class="sxs-lookup"><span data-stu-id="63b49-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="63b49-121">Skriv for at finde eller oprette mærker.</span><span class="sxs-lookup"><span data-stu-id="63b49-121">Type to find or create tags.</span></span>

<span data-ttu-id="63b49-122">Mærker føjes til enhedsvisningen og afspejles i listevisningen Enheder.</span><span class="sxs-lookup"><span data-stu-id="63b49-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="63b49-123">Du kan derefter bruge filteret Mærker til at få vist den relevante liste over enheder.</span><span class="sxs-lookup"><span data-stu-id="63b49-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="63b49-124">Du kan få mere at vide [under Opret og administrer enhedsmærker](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="63b49-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>