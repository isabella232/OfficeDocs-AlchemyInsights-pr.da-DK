---
title: Kontrollér automatiske opdateringer til Office-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747770"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="00897-102">Kontrollér automatiske opdateringer til Office-Apps</span><span class="sxs-lookup"><span data-stu-id="00897-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="00897-103">Opdateringer til Office-apps downloades som standard automatisk og anvendes i baggrunden uden brugerinput.</span><span class="sxs-lookup"><span data-stu-id="00897-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="00897-104">Administratorer kan dog styre, hvordan opdateringer anvendes ved hjælp af Office Update-indstillinger.</span><span class="sxs-lookup"><span data-stu-id="00897-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="00897-105">Opdater indstillinger gør det muligt for administratorer at aktivere eller deaktivere automatiske opdateringer, vise eller skjule knappen **Opdater nu** i Office, angive deadlines og meget mere.</span><span class="sxs-lookup"><span data-stu-id="00897-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="00897-106">Hvis du vil have mere at vide, skal du se:</span><span class="sxs-lookup"><span data-stu-id="00897-106">For detailed information, see:</span></span>

- [<span data-ttu-id="00897-107">Konfigurere opdateringsindstillinger for Office</span><span class="sxs-lookup"><span data-stu-id="00897-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="00897-108">Automatisk opdatering til Office er ikke aktiveret</span><span class="sxs-lookup"><span data-stu-id="00897-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="00897-109">Definer, hvordan Office opdateres, efter det er installeret</span><span class="sxs-lookup"><span data-stu-id="00897-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="00897-110">Hvis du vil gennemgå de eksisterende opdateringer, der er anvendt på en klientmaskine, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="00897-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="00897-111">Åbn registrerings Editor ved at gå til **Start**  >  **kørsel**af  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="00897-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="00897-112">Skift til følgende placering, og gennemse indstillingerne for Office Update:</span><span class="sxs-lookup"><span data-stu-id="00897-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="00897-113">a.</span><span class="sxs-lookup"><span data-stu-id="00897-113">a.</span></span> <span data-ttu-id="00897-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="00897-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="00897-115">b.</span><span class="sxs-lookup"><span data-stu-id="00897-115">b.</span></span> <span data-ttu-id="00897-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="00897-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="00897-117">**Bemærk!**  Hvis OfficeMgmtCOM-nøglen er angivet, får du muligvis vist meddelelsen "opdateringer administreres af din systemadministrator" i **Office**-  >  **kontoens**  >  **Office-opdateringer**.</span><span class="sxs-lookup"><span data-stu-id="00897-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="00897-118">Du kan finde flere oplysninger i [administrere opdateringer til microsoft 365-apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="00897-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  