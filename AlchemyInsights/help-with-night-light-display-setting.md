---
title: Hjælp til skærmindstillingen nattelys
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404397"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="4eed1-102">Hjælp til skærmindstillingen nattelys</span><span class="sxs-lookup"><span data-stu-id="4eed1-102">Help with the night light display setting</span></span>

<span data-ttu-id="4eed1-103">Hvis du vil have mere at vide om indstillinger for nattid, skal du se Angive [din skærm til nattid i Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="4eed1-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="4eed1-104">Hvis indstillingerne for nattelys er nedtonet i Indstillinger, skal du kontrollere din skærmdriver:</span><span class="sxs-lookup"><span data-stu-id="4eed1-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="4eed1-105">Klik på søgefeltet på proceslinjen, og **skriv Enhedshåndtering,** og vælg **derefter Enhedshåndtering** i søgeresultaterne.</span><span class="sxs-lookup"><span data-stu-id="4eed1-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="4eed1-106">Udvid **skærmkort.**</span><span class="sxs-lookup"><span data-stu-id="4eed1-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="4eed1-107">Funktionen nattelys er desværre ikke tilgængelig, hvis enheden bruger en DisplayLink-driver eller en Basic Display-driver.</span><span class="sxs-lookup"><span data-stu-id="4eed1-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="4eed1-108">Funktionen nattelys gør brug af den nyeste grafikteknologi, så det kan være nødvendigt at opdatere skærmdriveren:</span><span class="sxs-lookup"><span data-stu-id="4eed1-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="4eed1-109">Søg efter opdateringer ved at gå til **Opdatering**  >  **af**  >  **startindstillinger &**  >  **Sikkerhedsopdatering til Windows Update** for at søge efter  >  **opdateringer.**</span><span class="sxs-lookup"><span data-stu-id="4eed1-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="4eed1-110">ELLER</span><span class="sxs-lookup"><span data-stu-id="4eed1-110">OR</span></span>

- <span data-ttu-id="4eed1-111">Besøg hardwareproducentens supportwebsted for manuelt at downloade og installere de nyeste skærmdrivere.</span><span class="sxs-lookup"><span data-stu-id="4eed1-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="4eed1-112">Nulstil nattelys i registreringsdatabasen</span><span class="sxs-lookup"><span data-stu-id="4eed1-112">Reset night light in the registry</span></span>

<span data-ttu-id="4eed1-113">Hvis det ikke virker at opdatere din skærmdriver, skal du muligvis nulstille nattelys i registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="4eed1-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="4eed1-114">**Advarsel!** Dette fejlfindingstrin anbefales kun til erfarne brugere.</span><span class="sxs-lookup"><span data-stu-id="4eed1-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="4eed1-115">Der kan forekomme alvorlige problemer, hvis du redigerer registreringsdatabasen forkert.</span><span class="sxs-lookup"><span data-stu-id="4eed1-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="4eed1-116">For yderligere beskyttelse skal du sikkerhedskopiering af registreringsdatabasen, før du redigerer den, så du kan gendanne den, hvis der opstår problemer.</span><span class="sxs-lookup"><span data-stu-id="4eed1-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="4eed1-117">Skriv **regedit i søgefeltet,** og vælg derefter **Registreringseditor** i søgeresultaterne.</span><span class="sxs-lookup"><span data-stu-id="4eed1-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="4eed1-118">Gå til følgende registreringsdatabasenøgle:</span><span class="sxs-lookup"><span data-stu-id="4eed1-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="4eed1-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="4eed1-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="4eed1-120">Eksportér og slet derefter følgende undernøgle:$$windows.data.bluelightreangivelse.bluelightrestate</span><span class="sxs-lookup"><span data-stu-id="4eed1-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="4eed1-121">Eksportér og slet derefter følgende undernøgle:$$windows.data.bluelightrerettelse.settings</span><span class="sxs-lookup"><span data-stu-id="4eed1-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="4eed1-122">Genstart Windows, og kontrollér, om indstillingerne for nattelys er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="4eed1-122">Restart Windows and verify if the night light options are available.</span></span>


