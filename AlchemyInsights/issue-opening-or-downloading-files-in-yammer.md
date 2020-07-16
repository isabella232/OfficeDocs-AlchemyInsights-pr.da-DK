---
title: Problem med at åbne eller hente filer i Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148205"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="9ddf5-102">Problem med at åbne eller hente filer i Yammer</span><span class="sxs-lookup"><span data-stu-id="9ddf5-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="9ddf5-103">Klassisk Yammer understøtter flere muligheder for filoverførsler til meddelelser og grupper.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="9ddf5-104">Afhængigt af netværkskonfigurationen er filerne som standard lager i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="9ddf5-105">Filvælgeren i den nye Yammer understøtter endnu ikke alle de muligheder, der er tilgængelige i klassisk Yammer.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="9ddf5-106">En fremtidig opdatering vil tilføje yderligere funktioner.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-106">A future update will add additional features.</span></span> <span data-ttu-id="9ddf5-107">Du kan finde flere oplysninger [under Vedhæfte en fil eller et billede til et Yammer-samtaleindlæg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="9ddf5-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="9ddf5-108">**En fil kan ikke åbnes eller hentes**</span><span class="sxs-lookup"><span data-stu-id="9ddf5-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="9ddf5-109">En fil overføres muligvis til Yammer, men linker også til en fil i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="9ddf5-110">Hvis du vil foretage fejlfinding, skal du først bestemme filens placering.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="9ddf5-111">Hvis filen er blevet overført til Yammer, har den en \*.yammer.com URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="9ddf5-112">Sørg for, at påkrævede URL-adresser og IP-adresser er fjernet.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="9ddf5-113">Du kan finde flere oplysninger i blogindlægget [Brug af hårde kodede IP-adresser til Yammer anbefales ikke](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="9ddf5-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="9ddf5-114">Kontroller, om en bruger, der også er global administrator, kan hente filen.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="9ddf5-115">Hvis filen er privat, skal du muligvis bruge Privat indholdstilstand.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="9ddf5-116">Du kan finde flere oplysninger under [Overvåge privat indhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="9ddf5-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="9ddf5-117">**Gæster og filer på Yammer-netværksniveau i SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="9ddf5-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="9ddf5-118">[Gæster på netværksniveau i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruger ikke Azure AD B2B og er interne i Yammer-tjenesten, så de kan ikke få adgang til Yammer-filer, der er gemt i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="9ddf5-119">Opret en ekstern AAD B2B-bruger, der kan få adgang til dokumentbiblioteker i SharePoint Online ved hjælp af denne identitet.</span><span class="sxs-lookup"><span data-stu-id="9ddf5-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="9ddf5-120">Du kan finde oplysninger om fremtidig Azure AD B2B-gæstesupport i Yammer under [Support af gæster i Business-to-business (B2B) i Yammer Preview – Kundevilkår og ofte stillede spørgsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="9ddf5-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>