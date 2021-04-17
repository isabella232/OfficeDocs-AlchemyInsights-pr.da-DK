---
title: Fejlfinding af OneDrive går ned
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826193"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="1b71d-102">Fejlfinding af OneDrive går ned</span><span class="sxs-lookup"><span data-stu-id="1b71d-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="1b71d-103">Hvis OneDrive går ned gentagne gange, kan du prøve disse fejlfindingstrin:</span><span class="sxs-lookup"><span data-stu-id="1b71d-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="1b71d-104">**Sørg for, at registreringsdatabasenøgler ikke er angivet:**</span><span class="sxs-lookup"><span data-stu-id="1b71d-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="1b71d-105">Brug registreringseditoren til at navigere til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="1b71d-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="1b71d-106">Hvis DisableFileSyncNGSC er til stede og angivet til 1, skal du åbne nøglen og ændre værdien til 0.</span><span class="sxs-lookup"><span data-stu-id="1b71d-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="1b71d-107">Start OneDrive manuelt ved at gå til Start</span><span class="sxs-lookup"><span data-stu-id="1b71d-107">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="1b71d-109">, skriv OneDrive i søgefeltet, og klik derefter på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="1b71d-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="1b71d-110">**Nulstil OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="1b71d-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="1b71d-111">Bemærkninger:</span><span class="sxs-lookup"><span data-stu-id="1b71d-111">Notes:</span></span>

- <span data-ttu-id="1b71d-112">Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder din personlige OneDrive, hvis konfigureret).</span><span class="sxs-lookup"><span data-stu-id="1b71d-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="1b71d-113">Du mister ikke filer eller data ved at nulstille OneDrive på computeren.</span><span class="sxs-lookup"><span data-stu-id="1b71d-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="1b71d-114">**Sådan nulstiller du OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="1b71d-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="1b71d-115">Åbn dialogboksen Kør ved at trykke på Windows-tasten og R.</span><span class="sxs-lookup"><span data-stu-id="1b71d-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="1b71d-116">Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og tryk på OK.</span><span class="sxs-lookup"><span data-stu-id="1b71d-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="1b71d-117">Et kommandovindue vises muligvis kort.</span><span class="sxs-lookup"><span data-stu-id="1b71d-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="1b71d-118">Start OneDrive manuelt ved at gå til Start</span><span class="sxs-lookup"><span data-stu-id="1b71d-118">Manually launch OneDrive by going to Start</span></span> ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="1b71d-120">, skriv OneDrive i søgefeltet, og klik derefter på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="1b71d-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="1b71d-121">Bemærkninger:</span><span class="sxs-lookup"><span data-stu-id="1b71d-121">Notes:</span></span>

- <span data-ttu-id="1b71d-122">Hvis du havde valgt kun at synkronisere nogle mapper før nulstillingen, er du nødt til at gøre dette igen, når synkroniseringen er fuldført.</span><span class="sxs-lookup"><span data-stu-id="1b71d-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="1b71d-123">Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres til din computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)for at få flere   oplysninger.</span><span class="sxs-lookup"><span data-stu-id="1b71d-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="1b71d-124">Du skal gennemføre dette for dit personlige OneDrive og OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1b71d-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>