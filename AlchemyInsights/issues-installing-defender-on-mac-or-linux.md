---
title: Problemer med installation af Microsoft Defender på Mac eller Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539674"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="df52c-102">Problemer med installation af Microsoft Defender på Mac eller Linux</span><span class="sxs-lookup"><span data-stu-id="df52c-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="df52c-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="df52c-103">**Mac**</span></span>

- <span data-ttu-id="df52c-104">Sørg for, at systemkravene er opfyldt, før du Microsoft Defender ATP til Mac.</span><span class="sxs-lookup"><span data-stu-id="df52c-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="df52c-105">Du kan finde flere oplysninger [under Sådan installerer du Microsoft Defender ATP til Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="df52c-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="df52c-106">Gennemse oplysningerne i filen: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="df52c-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="df52c-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="df52c-107">**Linux**</span></span>

- <span data-ttu-id="df52c-108">Sørg for, at systemkravene er opfyldt, før du Microsoft Defender ATP til Linux.</span><span class="sxs-lookup"><span data-stu-id="df52c-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="df52c-109">Du kan finde flere oplysninger [under Sådan installerer du MDATP til Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="df52c-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="df52c-110">Hvis du vil bekræfte, MDATP tjeneste kører, skal du se [Installation mislykkedes.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="df52c-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="df52c-111">Hvis du vil foretage fejlfinding og løse problemer, hvis tjenesten ikke kører, skal du se Trin til fejlfinding, [hvis mdatp-tjenesten ikke kører.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="df52c-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="df52c-112">Du kan finde trin til at kontrollere klientkonfigurationen, som bekræfter produktets tilstand, og for at køre en registreringstest på EICAR-tekstfilen, under [Klientkonfiguration.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="df52c-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="df52c-113">**Bemærk!** Du kan finde en liste over understøttede filsystemer til aktivitet under [Microsoft Defender ATP til Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="df52c-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>