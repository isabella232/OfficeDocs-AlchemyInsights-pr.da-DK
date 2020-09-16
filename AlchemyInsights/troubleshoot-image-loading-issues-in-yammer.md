---
title: Fejlfinding på problemer med at indlæse billeder i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690237"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="bc17f-102">Fejlfinding på problemer med at indlæse billeder i Yammer</span><span class="sxs-lookup"><span data-stu-id="bc17f-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="bc17f-103">Når der opstår problemer med billeder og fil-eksempler i Yammer, kan du foretage fejlfinding ved at kontrollere, om problemet opstår for alle brugere, uanset om det sker på mobilenheder, og om det kan genskabes, når den vedhæftede fil overføres.</span><span class="sxs-lookup"><span data-stu-id="bc17f-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="bc17f-104">**Problemer med profilbilleder**</span><span class="sxs-lookup"><span data-stu-id="bc17f-104">**Profile photo issues**</span></span>  

<span data-ttu-id="bc17f-105">Hvis slutbrugerne logger på Yammer via Microsoft 365, skal de ændre deres profil, herunder deres profilbillede.</span><span class="sxs-lookup"><span data-stu-id="bc17f-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="bc17f-106">Hvis brugerne ikke har tilladelse til at oprette profilopdateringer, kan en administrator udføre opdateringen for brugeren.</span><span class="sxs-lookup"><span data-stu-id="bc17f-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="bc17f-107">Du kan finde flere oplysninger i [få vist og opdatere din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="bc17f-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="bc17f-108">Du kan finde oplysninger om profil redigering, herunder profilbilleder, under [ændre min Yammer-profil og-indstillinger](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="bc17f-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="bc17f-109">Opdaterede profil fotos synkroniseres anderledes end profil attributter.</span><span class="sxs-lookup"><span data-stu-id="bc17f-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="bc17f-110">Brugere skal logge på for at begynde at synkronisere deres profilbillede.</span><span class="sxs-lookup"><span data-stu-id="bc17f-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="bc17f-111">Hvis du vil have oplysninger, skal du se [brugerprofilbilleder, der er opdateret fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="bc17f-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="bc17f-112">Du kan finde oplysninger om bruger livscyklussen for Yammer under [administrere Yammer-brugere på tværs af deres livscyklus fra Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="bc17f-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="bc17f-113">Hvis du vil have mere at vide om, hvordan profil billed synkronisering fungerer i Microsoft 365, skal du se [oplysninger om synkronisering af profilbilleder i microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="bc17f-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="bc17f-114">**Dokument eksempler og problemer med miniaturebilleder**</span><span class="sxs-lookup"><span data-stu-id="bc17f-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="bc17f-115">Når filer eller billeder bliver sendt til Yammer, vises eksempelvisningerne muligvis ikke, fordi:</span><span class="sxs-lookup"><span data-stu-id="bc17f-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="bc17f-116">Filen er beskadiget og kan ikke behandles.</span><span class="sxs-lookup"><span data-stu-id="bc17f-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="bc17f-117">Filen er ikke for nylig blevet overført til SharePoint Online, eller Yammer har ugyldige metadata for andre årsager.</span><span class="sxs-lookup"><span data-stu-id="bc17f-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="bc17f-118">De URL-adresser, der kræves for at indlæse eksempelbillederne, blokeres.</span><span class="sxs-lookup"><span data-stu-id="bc17f-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="bc17f-119">Visningen af filen blev fjernet af brugeren før bogføringen.</span><span class="sxs-lookup"><span data-stu-id="bc17f-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="bc17f-120">Et tjeneste problem forhindrede, at der blev oprettet en forhåndsvisning.</span><span class="sxs-lookup"><span data-stu-id="bc17f-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="bc17f-121">**Bemærk!** Eksempler på links og filoverførsler fungerer muligvis anderledes.</span><span class="sxs-lookup"><span data-stu-id="bc17f-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="bc17f-122">Links til filer på internettet eller links, der kræver yderligere godkendelse, vises muligvis ikke korrekt.</span><span class="sxs-lookup"><span data-stu-id="bc17f-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="bc17f-123">Se [Vedhæft en fil eller et billede til en Yammer-meddelelse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="bc17f-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 