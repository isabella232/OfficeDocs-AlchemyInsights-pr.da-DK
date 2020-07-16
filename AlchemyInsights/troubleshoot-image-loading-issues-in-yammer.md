---
title: Fejlfinding i forbindelse med indlæsning af billeder i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148195"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="0c9a1-102">Fejlfinding i forbindelse med indlæsning af billeder i Yammer</span><span class="sxs-lookup"><span data-stu-id="0c9a1-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="0c9a1-103">Når der opstår problemer med billeder og eksempelvisninger af filer i Yammer, skal du foretage fejlfinding ved at kontrollere, om problemet opstår for alle brugere, om det opstår på mobilenheder, og om det er reproducerbart, når den vedhæftede fil overføres.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="0c9a1-104">**Problemer med profilfoto**</span><span class="sxs-lookup"><span data-stu-id="0c9a1-104">**Profile photo issues**</span></span>  

<span data-ttu-id="0c9a1-105">Hvis slutbrugerne logger på Yammer via Microsoft 365, skal de ændre deres profil, herunder deres profilbillede.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="0c9a1-106">Hvis brugerne ikke har tilladelse til at foretage profilopdateringer, kan en administrator foretage opdateringen for brugeren.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="0c9a1-107">Du kan finde flere oplysninger under [Få vist og opdatere din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="0c9a1-108">Du kan finde flere oplysninger om profilredigering, herunder profilbilleder, under [Ændre min Yammer-profil og mine indstillinger](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="0c9a1-109">Opdaterede profilbilleder synkroniseres anderledes end profilattributter.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="0c9a1-110">Brugerne skal logge på for at starte en synkronisering af deres profilbillede.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="0c9a1-111">Du kan finde flere oplysninger i [brugerprofilbilleder, der er opdateret fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="0c9a1-112">Du kan finde oplysninger om brugerlivscyklussen for Yammer under [Administrere Yammer-brugere i hele deres livscyklus fra Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="0c9a1-113">Du kan finde flere oplysninger om, hvordan synkronisering af profilbilleder fungerer i Microsoft 365, [under Oplysninger om synkronisering af profilbilleder i Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="0c9a1-114">**Problemer med dokumenteksempler og miniaturebilleder**</span><span class="sxs-lookup"><span data-stu-id="0c9a1-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="0c9a1-115">Når filer eller billeder sendes til Yammer, vises forhåndsvisninger muligvis ikke, fordi:</span><span class="sxs-lookup"><span data-stu-id="0c9a1-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="0c9a1-116">Filen er beskadiget og kan ikke behandles.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="0c9a1-117">Filen er ikke for nylig blevet overført til SharePoint Online, eller Yammer har ugyldige metadata af andre årsager.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="0c9a1-118">URL-adresser, der kræves til indlæsning af eksempelbillederne, blokeres.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="0c9a1-119">Fileksemplet blev fjernet af brugeren, før det blev slået op.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="0c9a1-120">Et serviceproblem forhindrede, at der blev genereret et eksempel.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="0c9a1-121">**Bemærk:** Forhåndsvisninger af links og filoverførsler kan opføre sig anderledes.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="0c9a1-122">Links til filer på internettet eller links, der kræver yderligere godkendelse, vises muligvis ikke korrekt.</span><span class="sxs-lookup"><span data-stu-id="0c9a1-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="0c9a1-123">Du kan finde flere oplysninger [under Vedhæfte en fil eller et billede til en Yammer-meddelelse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="0c9a1-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 