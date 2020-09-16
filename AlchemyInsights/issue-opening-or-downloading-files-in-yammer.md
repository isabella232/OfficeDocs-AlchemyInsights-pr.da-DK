---
title: Problem med at åbne eller hente filer i Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695643"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="eb7a3-102">Problem med at åbne eller hente filer i Yammer</span><span class="sxs-lookup"><span data-stu-id="eb7a3-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="eb7a3-103">Klassisk Yammer understøtter flere mulighederne for fil overførsler til meddelelser og grupper.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="eb7a3-104">Afhængigt af netværkskonfigurationen er filer som standard gemt i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="eb7a3-105">Valg af fil i ny Yammer understøtter endnu ikke alle de muligheder, der er tilgængelige i klassisk Yammer.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="eb7a3-106">En fremtidig opdatering vil tilføje yderligere funktioner.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-106">A future update will add additional features.</span></span> <span data-ttu-id="eb7a3-107">Hvis du vil have mere at vide, skal du se [vedhæfte en fil eller et billede til et Yammer-samtale indlæg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="eb7a3-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="eb7a3-108">**Kan ikke åbne eller downloade en fil**</span><span class="sxs-lookup"><span data-stu-id="eb7a3-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="eb7a3-109">En fil kan uploades til Yammer, men også oprette en kæde til en fil i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="eb7a3-110">For at foretage fejlfinding skal du først bestemme placeringen af filen.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="eb7a3-111">Hvis filen er blevet overført til Yammer, får den en \*. yammer.com-URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="eb7a3-112">Kontrollér, at de påkrævede URL-adresser og IP-adresser ikke er blokeret.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="eb7a3-113">Hvis du vil have flere oplysninger, kan du se blogindlægget [ved hjælp af hard coded IP-adresser til Yammer](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="eb7a3-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="eb7a3-114">Kontrollér, om en bruger, der også er en global administrator, kan downloade filen.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="eb7a3-115">Hvis filen er privat, skal du muligvis bruge privat indholds tilstand.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="eb7a3-116">Hvis du vil have mere at vide, skal du se [overvåge det private indhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="eb7a3-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="eb7a3-117">**Gæster og filer i Yammer-netværksniveau i SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="eb7a3-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="eb7a3-118">[Gæster på netværksniveau i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruger ikke Azure ad B2B og er interne for yammer-tjenesten, så de kan ikke få adgang til yammer-filer, der er gemt i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="eb7a3-119">Opret en ekstern AAD B2B-bruger, der kan få adgang til dokumentbiblioteker i SharePoint Online ved hjælp af den pågældende identitet.</span><span class="sxs-lookup"><span data-stu-id="eb7a3-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="eb7a3-120">Hvis du vil have mere at vide om fremtidig Azure AD B2B-gæste support i Yammer, skal du se [gæste support i Business-to-business (B2B) i Yammer preview – kunde vilkår og ofte stillede spørgsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="eb7a3-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>