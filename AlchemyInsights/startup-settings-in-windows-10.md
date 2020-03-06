---
title: Startindstillinger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408969"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="a8e37-102">Startindstillinger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="a8e37-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="a8e37-103">**Ændre, hvilke apps der kører automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="a8e37-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="a8e37-104">Gå til [Indstillinger > Apps > Start](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="a8e37-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="a8e37-105">Sørg for, at alle apps, du vil køre ved start, er **slået**til .</span><span class="sxs-lookup"><span data-stu-id="a8e37-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="a8e37-106">**Tilføje en app for at køre automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="a8e37-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="a8e37-107">Klik eller tryk på **Start,** og find den app, du vil køre ved start.</span><span class="sxs-lookup"><span data-stu-id="a8e37-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="a8e37-108">Højreklik på appen, klik på **Mere**, og klik derefter på **Åbn filplacering**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="a8e37-109">Dette åbner den placering, hvor genvejen til appen gemmes.</span><span class="sxs-lookup"><span data-stu-id="a8e37-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="a8e37-110">Hvis der ikke er nogen indstilling for Placering af Åbn fil, betyder det, at appen ikke kan køre ved start.</span><span class="sxs-lookup"><span data-stu-id="a8e37-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="a8e37-111">Når filplaceringen er åben, skal du trykke på **Windows-tasten + R**, skrive **shell:startup**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="a8e37-112">Derved åbnes mappen Start.</span><span class="sxs-lookup"><span data-stu-id="a8e37-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="a8e37-113">Kopiér og indsæt genvejen til appen fra filplaceringen i mappen Start.</span><span class="sxs-lookup"><span data-stu-id="a8e37-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="a8e37-114">**Avancerede startindstillinger (herunder fejlsikret tilstand, UEFI-indstillinger og opstart fra en anden enhed)**</span><span class="sxs-lookup"><span data-stu-id="a8e37-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="a8e37-115">Gem dit arbejde, og luk alle åbne dokumenter, da disse trin genstarter pc'en.</span><span class="sxs-lookup"><span data-stu-id="a8e37-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="a8e37-116">Gå til [Indstillinger > Opdatering & Genoprettelse > sikkerhedsgendannelse](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="a8e37-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="a8e37-117">Klik på **Genstart nu**under **Avanceret start**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="a8e37-118">Når din pc er genstartet til skærmbilledet Vælg en indstilling:</span><span class="sxs-lookup"><span data-stu-id="a8e37-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="a8e37-119">Hvis du vil starte fra en enhed som et USB-drev, skal du klikke på **Brug en enhed**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="a8e37-120">Hvis du vil angive UEFI-indstillingerne (også kaldet BIOS-opsætning), skal du klikke **på Fejlfinding > Avancerede indstillinger > UEFI-firmwareindstillinger**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="a8e37-121">Hvis du vil angive fejlsikret tilstand eller ændre avancerede startindstillinger, skal du klikke på **Fejlfinding > Avancerede indstillinger > Startindstillinger**og derefter klikke på **Genstart**.</span><span class="sxs-lookup"><span data-stu-id="a8e37-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="a8e37-122">Du kan blive bedt om at angive [bitlockergenoprettelsesnøglen](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="a8e37-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="a8e37-123">Når pc'en er genstartet igen, skal du klikke på den startindstilling, du vil bruge.</span><span class="sxs-lookup"><span data-stu-id="a8e37-123">After your PC restarts again, click the startup setting you want to use.</span></span>