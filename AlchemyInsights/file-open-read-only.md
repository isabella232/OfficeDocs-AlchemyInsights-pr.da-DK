---
title: Åbn fil som skrivebeskyttet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745571"
---
# <a name="file-open-read-only"></a><span data-ttu-id="2c8b8-102">Åbn fil som skrivebeskyttet</span><span class="sxs-lookup"><span data-stu-id="2c8b8-102">File open read-only</span></span>

<span data-ttu-id="2c8b8-103">Du kan finde frem til, at når du åbner filer, åbnes de som skrivebeskyttede.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="2c8b8-104">I nogle tilfælde er dette en ekstra sikkerhed, f. eks når du åbner filer fra internettet og andre gange, kan det skyldes en indstilling, der kan ændres.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="2c8b8-105">Her er nogle scenarier, hvor en fil åbner i skrivebeskyttet tilstand og nogle trin, du kan gøre for at ændre det.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="2c8b8-106">**Mit antivirusprogram er skyld i, at de åbner skrivebeskyttede**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="2c8b8-107">Nogle antivirusprogrammer beskytter dig muligvis mod potentielt usikre filer ved at åbne dem i skrivebeskyttet tilstand.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="2c8b8-108">Du skal muligvis kontakte din antivirusudbyder for at få mere at vide om, hvordan du justerer disse indstillinger.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="2c8b8-109">BitDefender har som eksempelindhold til tilføjelse af programundtagelser her: [Sådan tilføjer du programmer eller proces undtagelser i BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="2c8b8-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="2c8b8-110">**Er filegenskaberne indstillet til skrivebeskyttede?**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="2c8b8-111">Du kan kontrollere egenskaberne for filen ved at højreklikke på filen og vælge egenskaber.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="2c8b8-112">Hvis skrivebeskyttelsesattributten er markeret, kan du fjerne markeringen af den og klikke på OK.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="2c8b8-113">**Indholdet er i beskyttet visning**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="2c8b8-114">Filer fra internettet og andre potentielt usikre placeringer kan indeholde virus, orme eller andre typer skadelig software, der kan skade din computer.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="2c8b8-115">Dette er også normalt tilfældet med vedhæftede filer i mails eller filer, du har hentet.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="2c8b8-116">Filer fra disse potentielt usikre placeringer åbnes i beskyttet visning for at hjælpe med at beskytte din computer.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="2c8b8-117">Ved hjælp af beskyttet visning kan du læse en fil og se dens indhold, mens du reducerer risiciene.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="2c8b8-118">Du kan finde flere oplysninger om beskyttet visning, og hvordan du ændrer indstillinger, i denne artikel: [Hvad er beskyttet visning?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="2c8b8-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="2c8b8-119">**Er OneDrive fuld?**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="2c8b8-120">Hvis filen er gemt på OneDrive, og din OneDrive-lagerplads er fuld, kan du ikke gemme dokumentet, før du er under det tildelte område.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="2c8b8-121">Du kan kontrollere din ledige plads på OneDrive ved at klikke på OneDrive-ikonet i meddelelses Center og vælge Administrer lager, eller du kan gå til [https://onedrive.live.com](https://onedrive.live.com) , logge på og notere mængden af anvendt plads nederst til venstre på skærmen.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="2c8b8-122">**Er Office aktiveret?**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="2c8b8-123">Hvis Office ikke er aktiveret, eller hvis dit abonnement er udløbet, kan du være i skrivebeskyttet tilstand med reducerede funktioner.</span><span class="sxs-lookup"><span data-stu-id="2c8b8-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="2c8b8-124">Hvis du vil have mere at vide om, hvordan du aktiverer Office, skal du se: [fejl i forbindelse med produkt og aktivering af licens i Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="2c8b8-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="2c8b8-125">**Hvis alt andet mislykkes...**</span><span class="sxs-lookup"><span data-stu-id="2c8b8-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="2c8b8-126">Prøv at genstarte computeren</span><span class="sxs-lookup"><span data-stu-id="2c8b8-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="2c8b8-127">Installer Office-opdateringer</span><span class="sxs-lookup"><span data-stu-id="2c8b8-127">Install Office updates</span></span>
    
- <span data-ttu-id="2c8b8-128">Udføre en online reparation af Office</span><span class="sxs-lookup"><span data-stu-id="2c8b8-128">Perform an Online repair of Office</span></span>
    

