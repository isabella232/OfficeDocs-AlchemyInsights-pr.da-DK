---
title: Styre automatiske opdateringer til Office-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438992"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="791a6-102">Styre automatiske opdateringer til Office-apps</span><span class="sxs-lookup"><span data-stu-id="791a6-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="791a6-103">Opdateringer til Office Apps hentes som standard automatisk og anvendes i baggrunden uden brugerindgriben.</span><span class="sxs-lookup"><span data-stu-id="791a6-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="791a6-104">Administratorer kan dog styre, hvordan opdateringer anvendes, ved hjælp af Office Update-indstillinger.</span><span class="sxs-lookup"><span data-stu-id="791a6-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="791a6-105">Opdateringsindstillinger giver administratorer mulighed for at aktivere eller deaktivere automatiske opdateringer, **vise eller skjule knappen Opdater** nu i Office, angive opdateringsfrister og meget mere.</span><span class="sxs-lookup"><span data-stu-id="791a6-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="791a6-106">Yderligere oplysninger finder du i:</span><span class="sxs-lookup"><span data-stu-id="791a6-106">For detailed information, see:</span></span>

- [<span data-ttu-id="791a6-107">Konfigurere opdateringsindstillinger for Office</span><span class="sxs-lookup"><span data-stu-id="791a6-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="791a6-108">Automatisk opdatering til Office er ikke aktiveret</span><span class="sxs-lookup"><span data-stu-id="791a6-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="791a6-109">Definere, hvordan Office opdateres, når det er installeret</span><span class="sxs-lookup"><span data-stu-id="791a6-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="791a6-110">FÃ ̧lg disse trin for at gennemse de eksisterende opdateringerindstillinger, der er anvendt på en klientcomputer:</span><span class="sxs-lookup"><span data-stu-id="791a6-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="791a6-111">Åbn Registreringseditor ved at gå **til Start**  >  **Kør**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="791a6-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="791a6-112">Skift til følgende placering, og gennemse indstillingerne for Office Update:</span><span class="sxs-lookup"><span data-stu-id="791a6-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="791a6-113">a.</span><span class="sxs-lookup"><span data-stu-id="791a6-113">a.</span></span> <span data-ttu-id="791a6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="791a6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="791a6-115">b.</span><span class="sxs-lookup"><span data-stu-id="791a6-115">b.</span></span> <span data-ttu-id="791a6-116">Klik påRun\Konfiguration</span><span class="sxs-lookup"><span data-stu-id="791a6-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="791a6-117">**Bemærk:**  Hvis OfficeMgmtCOM-nøglen er angivet, vises meddelelsen "Opdateringer administreres af systemadministratoren" i **Office**  >  **Office-kontoopdateringer**  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="791a6-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="791a6-118">Du kan finde flere oplysninger [under Administrere opdateringer til Microsoft 365 Apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="791a6-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  