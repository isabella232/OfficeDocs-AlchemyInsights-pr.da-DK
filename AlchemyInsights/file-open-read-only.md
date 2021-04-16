---
title: Fil åben som skrivebeskyttet
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813178"
---
# <a name="file-open-read-only"></a><span data-ttu-id="6380d-102">Fil åben som skrivebeskyttet</span><span class="sxs-lookup"><span data-stu-id="6380d-102">File open read-only</span></span>

<span data-ttu-id="6380d-103">Når du åbner filer, vil du måske opleve, at de åbnes som skrivebeskyttede.</span><span class="sxs-lookup"><span data-stu-id="6380d-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="6380d-104">I nogle tilfælde er dette af sikkerhedsmæssige hensyn, f.eks. når du åbner filer fra internettet, og andre gange kan det skyldes en indstilling, der kan ændres.</span><span class="sxs-lookup"><span data-stu-id="6380d-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="6380d-105">Her er nogle scenarier, hvor en fil åbnes som skrivebeskyttet, og nogle trin, du kan følge for at ændre dette.</span><span class="sxs-lookup"><span data-stu-id="6380d-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="6380d-106">**Mit antivirusprogram er skyld i, at de åbner i skrivebeskyttet stand**</span><span class="sxs-lookup"><span data-stu-id="6380d-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="6380d-107">Nogle antivirusprogrammer kan beskytte dig mod potentielt usikre filer ved at åbne dem som skrivebeskyttede.</span><span class="sxs-lookup"><span data-stu-id="6380d-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="6380d-108">Du skal muligvis kontakte din antivirusudbyder for at få mere at vide om, hvordan du justerer disse indstillinger.</span><span class="sxs-lookup"><span data-stu-id="6380d-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="6380d-109">BitDefender har f.eks. indhold om tilføjelse af programudetagelser her: Sådan tilføjes program- eller procesudetagelser [i Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="6380d-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="6380d-110">**Er filegenskaberne angivet til skrivebeskyttet?**</span><span class="sxs-lookup"><span data-stu-id="6380d-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="6380d-111">Du kan kontrollere filegenskaberne ved at højreklikke på filen og vælge Egenskaber.</span><span class="sxs-lookup"><span data-stu-id="6380d-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="6380d-112">Hvis attributten Skrivebeskyttet er markeret, kan du fjerne markeringen og klikke på OK.</span><span class="sxs-lookup"><span data-stu-id="6380d-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="6380d-113">**Indholdet er i beskyttet visning**</span><span class="sxs-lookup"><span data-stu-id="6380d-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="6380d-114">Filer fra internettet og fra andre potentielt usikre placeringer kan indeholde virus, orme eller andre typer malware, der kan skade din computer.</span><span class="sxs-lookup"><span data-stu-id="6380d-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="6380d-115">Dette er også ofte tilfældet med vedhæftede filer i mails eller filer, du har downloadet.</span><span class="sxs-lookup"><span data-stu-id="6380d-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="6380d-116">For at beskytte din computer åbnes filer fra disse potentielt usikre placeringer i Beskyttet visning.</span><span class="sxs-lookup"><span data-stu-id="6380d-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="6380d-117">Med Beskyttet visning kan du læse en fil og se indholdet samtidig med, at du reducerer risiciene.</span><span class="sxs-lookup"><span data-stu-id="6380d-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="6380d-118">Du kan finde flere oplysninger om Beskyttet visning, og hvordan du ændrer indstillingerne, i denne artikel: [Hvad er Beskyttet visning?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="6380d-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="6380d-119">**Er OneDrive fuld?**</span><span class="sxs-lookup"><span data-stu-id="6380d-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="6380d-120">Hvis filen er gemt på OneDrive, og din OneDrive-lagerplads er fuld, kan du ikke gemme dokumentet, før du er inden for den tildelte plads.</span><span class="sxs-lookup"><span data-stu-id="6380d-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="6380d-121">Du kan kontrollere din ledige plads på OneDrive ved at klikke på OneDrive-ikonet i meddelelsescenteret og vælge Administrer lager, eller du kan gå til , logge på og notere mængden af anvendt plads nederst til venstre på [https://onedrive.live.com](https://onedrive.live.com) skærmen.</span><span class="sxs-lookup"><span data-stu-id="6380d-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="6380d-122">**Er Office aktiveret?**</span><span class="sxs-lookup"><span data-stu-id="6380d-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="6380d-123">Hvis Office ikke er aktiveret, eller hvis dit abonnement er udløbet, kan du være i den skrivebeskyttede tilstand Begrænset funktionalitet.</span><span class="sxs-lookup"><span data-stu-id="6380d-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="6380d-124">Hvis du vil have mere at vide om, hvordan du aktiverer Office, skal du [se: Fejl i forbindelse](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)med produkt og aktivering uden licens .</span><span class="sxs-lookup"><span data-stu-id="6380d-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="6380d-125">**Hvis intet andet virker...**</span><span class="sxs-lookup"><span data-stu-id="6380d-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="6380d-126">Prøv at genstarte computeren</span><span class="sxs-lookup"><span data-stu-id="6380d-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="6380d-127">Installér Office-opdateringer</span><span class="sxs-lookup"><span data-stu-id="6380d-127">Install Office updates</span></span>
    
- <span data-ttu-id="6380d-128">Udføre en onlinereparation af Office</span><span class="sxs-lookup"><span data-stu-id="6380d-128">Perform an Online repair of Office</span></span>
    

