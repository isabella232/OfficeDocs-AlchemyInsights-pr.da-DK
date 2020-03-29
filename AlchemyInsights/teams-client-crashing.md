---
title: Går Teams-klient ned?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030537"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="94e79-102">Går Teams-klient ned?</span><span class="sxs-lookup"><span data-stu-id="94e79-102">Teams client crashing?</span></span>

<span data-ttu-id="94e79-103">Hvis din Teams-klient går ned, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="94e79-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="94e79-104">Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="94e79-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="94e79-105">Sørg for, at alle [Office 365-webadresser og -adresseområder](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="94e79-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="94e79-106">Log på med din administratorkonto, og kontroller dit [Dashboard for tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen afbrydelse eller forringelse af tjenesten.</span><span class="sxs-lookup"><span data-stu-id="94e79-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="94e79-107">Som sidste trin kan du forsøge at rydde Teams-klientcachen:</span><span class="sxs-lookup"><span data-stu-id="94e79-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="94e79-108">Afslut Microsoft Teams-skrivebordsklienten helt.</span><span class="sxs-lookup"><span data-stu-id="94e79-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="94e79-109">Du kan højreklikke på **Teams** fra ikonbakken, og klikke på **Afslut**, eller køre Jobliste og afslutte processen helt.</span><span class="sxs-lookup"><span data-stu-id="94e79-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="94e79-110">Gå til Stifinder, og skriv %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="94e79-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="94e79-111">Når du er i kataloget, får du vist nogle af følgende mapper:</span><span class="sxs-lookup"><span data-stu-id="94e79-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="94e79-112">I **Programcache** skal du gå til Cache og slette alle filer på cacheplaceringen: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="94e79-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="94e79-113">Inde fra **Blob_storage** skal du slette alle filer: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="94e79-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="94e79-114">Inde fra **Cache** skal du slette alle filer: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="94e79-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="94e79-115">Inde fra **databaser** skal du slette alle filer: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="94e79-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="94e79-116">Inde fra **GPUCache** skal du slette alle filer: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="94e79-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="94e79-117">Inde fra **IndexedDB** skal du slette .db-filen: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="94e79-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="94e79-118">Inde fra **Lokalt lager** skal du slette alle filer: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="94e79-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="94e79-119">Til sidst skal du inde fra **tmp** slette en hvilken som helst fil: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="94e79-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="94e79-120">Genstart din Teams-klient.</span><span class="sxs-lookup"><span data-stu-id="94e79-120">Restart your Teams client.</span></span>
