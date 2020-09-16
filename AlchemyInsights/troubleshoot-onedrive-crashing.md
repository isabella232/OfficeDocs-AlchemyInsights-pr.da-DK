---
title: Fejlfinding af OneDrive-nedbrud
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664992"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="f253e-102">Fejlfinding af OneDrive-nedbrud</span><span class="sxs-lookup"><span data-stu-id="f253e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="f253e-103">Hvis OneDrive gentagne gange går ned, kan du prøve disse trin til fejlfinding:</span><span class="sxs-lookup"><span data-stu-id="f253e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="f253e-104">**Kontrollér, at registreringsdatabasenøgler ikke er angivet:**</span><span class="sxs-lookup"><span data-stu-id="f253e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="f253e-105">Ved hjælp af registrerings Editor skal du gå til HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="f253e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="f253e-106">Hvis DisableFileSyncNGSC er angivet og indstillet til 1, skal du åbne nøglen og ændre værdien til 0.</span><span class="sxs-lookup"><span data-stu-id="f253e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="f253e-107">Start OneDrive manuelt ved at gå til start</span><span class="sxs-lookup"><span data-stu-id="f253e-107">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f253e-109">, Skriv OneDrive i søgefeltet, og klik derefter på OneDrive-programmet på computeren.</span><span class="sxs-lookup"><span data-stu-id="f253e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f253e-110">**Nulstil OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f253e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="f253e-111">Vejledningen</span><span class="sxs-lookup"><span data-stu-id="f253e-111">Notes:</span></span>

- <span data-ttu-id="f253e-112">Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder dit personlige OneDrive, hvis det er konfigureret).</span><span class="sxs-lookup"><span data-stu-id="f253e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="f253e-113">Du mister ikke filer eller data ved at nulstille OneDrive på computeren.</span><span class="sxs-lookup"><span data-stu-id="f253e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="f253e-114">**Sådan nulstilles OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f253e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="f253e-115">Åbn en kørsels dialogboks ved at trykke på Windows-tasten og R.</span><span class="sxs-lookup"><span data-stu-id="f253e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="f253e-116">Skriv% localappdata% \Microsoft\OneDrive\onedrive.exe/reset, og tryk på OK.</span><span class="sxs-lookup"><span data-stu-id="f253e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="f253e-117">Et kommandovindue vises muligvis kortvarigt.</span><span class="sxs-lookup"><span data-stu-id="f253e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="f253e-118">Start OneDrive manuelt ved at gå til start</span><span class="sxs-lookup"><span data-stu-id="f253e-118">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f253e-120">, Skriv OneDrive i søgefeltet, og klik derefter på OneDrive-programmet på computeren.</span><span class="sxs-lookup"><span data-stu-id="f253e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f253e-121">Vejledningen</span><span class="sxs-lookup"><span data-stu-id="f253e-121">Notes:</span></span>

- <span data-ttu-id="f253e-122">Hvis du har valgt kun at synkronisere nogle mapper før nulstillingen, skal du gøre det igen, når synkroniseringen er fuldført.</span><span class="sxs-lookup"><span data-stu-id="f253e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="f253e-123">Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres med din computer for at](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="f253e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="f253e-124">Du skal fuldføre dette for dit personlige OneDrive og OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f253e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>