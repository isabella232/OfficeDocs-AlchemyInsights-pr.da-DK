---
title: Føj Microsoft Edge til Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194476"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="0146e-102">Føj Microsoft Edge til Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0146e-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="0146e-103">For at kunne installere, konfigurere, overvåge og beskytte Microsoft Edge til Windows 10 skal du først føje det til Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0146e-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="0146e-104">Intune understøtter Microsoft Edge 77 og nyere versioner.</span><span class="sxs-lookup"><span data-stu-id="0146e-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="0146e-105">Intune registrerer alle eksisterende installationer af Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="0146e-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="0146e-106">Hvis Microsoft Edge er installeret i brugerkontekst, overskriver en systeminstallation installationen i brugerkontekst.</span><span class="sxs-lookup"><span data-stu-id="0146e-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="0146e-107">Hvis Microsoft Edge er installeret i systemkontekst, rapporteres om installationens succes.</span><span class="sxs-lookup"><span data-stu-id="0146e-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="0146e-108">Forudinstalleret Microsoft Edge 77 og nyere versioner for alle kanaler i brugerkontekst overskrives med Microsoft Edge installeret i systemkontekst.</span><span class="sxs-lookup"><span data-stu-id="0146e-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="0146e-109">**Forudsætninger**</span><span class="sxs-lookup"><span data-stu-id="0146e-109">**Prerequisite**</span></span>

<span data-ttu-id="0146e-110">Windows 10 version 1709 eller nyere versioner</span><span class="sxs-lookup"><span data-stu-id="0146e-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="0146e-111">**Trin til at føje Edge til Intune**</span><span class="sxs-lookup"><span data-stu-id="0146e-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="0146e-112">[Konfigurer appen i Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="0146e-113">[Konfigurere appoplysningerne.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="0146e-114">[Konfigurer appindstillingerne.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="0146e-115">[Vælg områdemærkerne (valgfrit).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="0146e-116">[Tilføj appen.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="0146e-117">Du kan finde mere hjælp under [Fejlfinding.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0146e-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




