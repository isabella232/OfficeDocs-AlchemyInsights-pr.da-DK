---
title: Fejlfinding i forbindelse med nedbrud i OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748796"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e6c40-102">Fejlfinding i forbindelse med nedbrud i OneDrive</span><span class="sxs-lookup"><span data-stu-id="e6c40-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e6c40-103">Hvis OneDrive gentagne gange går ned, kan du prøve disse fejlfindingstrin:</span><span class="sxs-lookup"><span data-stu-id="e6c40-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e6c40-104">**Kontroller, at registreringsdatabasenøgler ikke er angivet:**</span><span class="sxs-lookup"><span data-stu-id="e6c40-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e6c40-105">Brug Registreringseditor til at navigere til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e6c40-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e6c40-106">Hvis DisableFileSyncNGSC er til stede og indstillet til 1, skal du åbne nøglen og ændre værdien til 0.</span><span class="sxs-lookup"><span data-stu-id="e6c40-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e6c40-107">Start OneDrive manuelt ved at gå til Start</span><span class="sxs-lookup"><span data-stu-id="e6c40-107">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e6c40-109">, skal du skrive OneDrive i søgefeltet og derefter klikke på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="e6c40-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e6c40-110">**Nulstil OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e6c40-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e6c40-111">Noter:</span><span class="sxs-lookup"><span data-stu-id="e6c40-111">Notes:</span></span>

- <span data-ttu-id="e6c40-112">Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder dit personlige OneDrive, hvis konfigureret).</span><span class="sxs-lookup"><span data-stu-id="e6c40-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e6c40-113">Du mister ikke filer eller data ved at nulstille OneDrive på din computer.</span><span class="sxs-lookup"><span data-stu-id="e6c40-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e6c40-114">**Sådan nulstilles OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e6c40-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e6c40-115">Åbn dialogboksen Kør ved at trykke på Windows-tasten og R.</span><span class="sxs-lookup"><span data-stu-id="e6c40-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e6c40-116">Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og tryk på OK.</span><span class="sxs-lookup"><span data-stu-id="e6c40-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e6c40-117">Der vises muligvis et kommandovindue kortvarigt.</span><span class="sxs-lookup"><span data-stu-id="e6c40-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e6c40-118">Start OneDrive manuelt ved at gå til Start</span><span class="sxs-lookup"><span data-stu-id="e6c40-118">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e6c40-120">, skal du skrive OneDrive i søgefeltet og derefter klikke på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="e6c40-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e6c40-121">Noter:</span><span class="sxs-lookup"><span data-stu-id="e6c40-121">Notes:</span></span>

- <span data-ttu-id="e6c40-122">Hvis du havde valgt kun at synkronisere nogle mapper før nulstillingen, skal du gøre det igen, når synkroniseringen er fuldført.</span><span class="sxs-lookup"><span data-stu-id="e6c40-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e6c40-123">Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres til computeren](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)for at få flere   oplysninger.</span><span class="sxs-lookup"><span data-stu-id="e6c40-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e6c40-124">Du skal udfylde dette for dit personlige OneDrive og OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e6c40-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>