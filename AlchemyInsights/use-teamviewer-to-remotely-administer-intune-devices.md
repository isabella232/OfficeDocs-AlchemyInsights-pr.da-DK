---
title: Brug TeamViewer til fjernadministrering af Intune-enheder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554841"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="42a83-102">Brug TeamViewer til fjernadministrering af Intune-enheder</span><span class="sxs-lookup"><span data-stu-id="42a83-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="42a83-103">Enheder, der administreres af Intune, kan fjernadministreres ved hjælp [af TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="42a83-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="42a83-104">Hvis du vil administrere Intune ved hjælp af TeamViewer, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="42a83-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="42a83-105">Begynd med at indhente legitimationsoplysninger fra TeamViewer for at konfigurere TeamViewer Connector på Intune.</span><span class="sxs-lookup"><span data-stu-id="42a83-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="42a83-106">Dette gør det muligt for administratoren at angive legitimationsoplysninger i TeamViewer Connector-brugergrænsefladen under Enheder, en engangshandling for at oprette forbindelsen mellem Intune og TeamViewer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="42a83-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="42a83-107">**Del 1: Start en session med en ekstern enhed**</span><span class="sxs-lookup"><span data-stu-id="42a83-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="42a83-108">Vælg **den enhed**, du vil starte en fjernsession med, under Alle enheder .</span><span class="sxs-lookup"><span data-stu-id="42a83-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="42a83-109">Fra **... Mere**, vælg **Ny fjernsupportsession**.</span><span class="sxs-lookup"><span data-stu-id="42a83-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="42a83-110">Vælg **Ja for** at bekræfte, at du vil oprette en fjernsession.</span><span class="sxs-lookup"><span data-stu-id="42a83-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="42a83-111">Når anmodningen "Igangsættelse af en ny fjernsession" er bekræftet af TeamViewer-tjenesten, får du vist en mulighed for **at starte fjernsupport** under oplysningerne i ruden Oversigt (eller Essentials) for enheden.</span><span class="sxs-lookup"><span data-stu-id="42a83-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="42a83-112">Vælg **Se mere** for at udvide ruden og få vist status for Fjernsupport.</span><span class="sxs-lookup"><span data-stu-id="42a83-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="42a83-113">Vælg **Start fjernsession** for at starte sessionen på administratorsiden.</span><span class="sxs-lookup"><span data-stu-id="42a83-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="42a83-114">Vælg at hente den binære TeamViewer (Windows), og vælg **Kør**.</span><span class="sxs-lookup"><span data-stu-id="42a83-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="42a83-115">**Bemærk:** Du kan ignorere enhver webbrowserside, der er åbnet på TeamViewer-webstedet.</span><span class="sxs-lookup"><span data-stu-id="42a83-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="42a83-116">Bekræft anmodningen om, at TeamViewer-appen skal foretage ændringer på enheden (kun Windows).</span><span class="sxs-lookup"><span data-stu-id="42a83-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="42a83-117">TeamViewer-appen starter og indeholder sessionskoden for at godkende forbindelsen til fjernenheden.</span><span class="sxs-lookup"><span data-stu-id="42a83-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="42a83-118">**Del 2: På den enhed, der er målrettet til en fjernsession**</span><span class="sxs-lookup"><span data-stu-id="42a83-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="42a83-119">Åbn Intune-firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="42a83-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="42a83-120">Se efter et meddelelsesflag: "It-administratoren anmoder om kontrol af denne enhed til en fjernsupportsession", og vælg meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="42a83-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="42a83-121">Vælg at downloade TeamViewer-programmet, eller bekræft download af TeamViewer-appen fra App Store, og vælg **Kør**.</span><span class="sxs-lookup"><span data-stu-id="42a83-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="42a83-122">**Bemærk:** Du kan ignorere enhver webbrowserside, der er åbnet på TeamViewer-webstedet.</span><span class="sxs-lookup"><span data-stu-id="42a83-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="42a83-123">Bekræft anmodningen om, at TeamViewer-appen skal foretage ændringer på enheden (kun Windows).</span><span class="sxs-lookup"><span data-stu-id="42a83-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="42a83-124">TeamViewer-appen starter og indeholder sessionskoden for at godkende forbindelsen til fjernenheden.</span><span class="sxs-lookup"><span data-stu-id="42a83-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="42a83-125">Et pop op-vindue bliver spurgt, om du vil tillade, at sessionen starter.</span><span class="sxs-lookup"><span data-stu-id="42a83-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="42a83-126">**Bemærk:** De sessionskoder, der genereres af TeamViewer-tjenesten, bruges kun én gang.</span><span class="sxs-lookup"><span data-stu-id="42a83-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="42a83-127">Hvis du mister forbindelsen, skal du:</span><span class="sxs-lookup"><span data-stu-id="42a83-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="42a83-128">Luk forekomsten af TeamViewer-appen på fjernenheden og på administratorarbejdsstationen.</span><span class="sxs-lookup"><span data-stu-id="42a83-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="42a83-129">Luk firmaportalen på fjernenheden.</span><span class="sxs-lookup"><span data-stu-id="42a83-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="42a83-130">Start en ny "Ny fjernsupportsession" fra administrationsportalen.</span><span class="sxs-lookup"><span data-stu-id="42a83-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="42a83-131">Åbn firmaportalen på fjernenheden igen for at modtage den nye meddelelse.</span><span class="sxs-lookup"><span data-stu-id="42a83-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="42a83-132">Download og åbn TeamViewer-appen på både fjernenheden og administratorarbejdsstationen som før.</span><span class="sxs-lookup"><span data-stu-id="42a83-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>