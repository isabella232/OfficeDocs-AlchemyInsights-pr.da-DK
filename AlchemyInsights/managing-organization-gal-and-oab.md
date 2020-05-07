---
title: Administrer organisations globale adresseliste og offlineadressekartotek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022438"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="9d612-102">Administrer organisations globale adresseliste (GAL) og offlineadressekartotek (OAB)</span><span class="sxs-lookup"><span data-stu-id="9d612-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="9d612-103">En Global adresseliste (GAL) er en liste over mailaktiverede objekter (enhver type modtager, der kan modtage mail) i organisationen.</span><span class="sxs-lookup"><span data-stu-id="9d612-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="9d612-104">En GAL oprettes automatisk i enhver organisation.</span><span class="sxs-lookup"><span data-stu-id="9d612-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="9d612-105">Du kan oprette yderligere globale adresselister for at adskille brugerne efter organisation eller sted, men en enkelt bruger kan kun se og bruge én global adresseliste ad gangen.</span><span class="sxs-lookup"><span data-stu-id="9d612-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="9d612-106">Nogle mailklienter, f. eks. Outlook til Windows, henter den globale adresseliste til offlinebrug..</span><span class="sxs-lookup"><span data-stu-id="9d612-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="9d612-107">Dette kaldes et offlineadressekartotek (OAB).</span><span class="sxs-lookup"><span data-stu-id="9d612-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="9d612-108">I Exchange Online opdateres et offlineadressekartotek kun én gang hver 8. time, og derefter skal klienter hente den for at opdatere deres lokale kopi af offlineadressekartoteket.</span><span class="sxs-lookup"><span data-stu-id="9d612-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="9d612-109">Enhver modtagerændring skal først kunne ses i den globale adresseliste for at kommer over i offlineadressekartoteket.</span><span class="sxs-lookup"><span data-stu-id="9d612-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="9d612-110">Her er nogle af de mest almindelige procedurer for global adresseliste og offlineadressekartoteket:</span><span class="sxs-lookup"><span data-stu-id="9d612-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="9d612-111">Af en række forskellige årsager kan det være en god ide, at nogle objekter skjules fra den globale adresseliste.</span><span class="sxs-lookup"><span data-stu-id="9d612-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="9d612-112">Se [Skjul modtagere fra adresselister](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="9d612-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="9d612-113">Hvis du har brug for at give bestemte grupper af brugere brugerdefinerede visninger af virksomhedens globale adresseliste, skal du se [Politikker for adressekartotek i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="9d612-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="9d612-114">[Opret en global adresseliste i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), og få mere at vide om, hvordan du arbejder med tilladelser for globale adresseliste, under [Adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="9d612-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="9d612-115">Bemærk, at hvis du opretter nye globale adresselister, kan det også være en god ide at oprette et nyt offlineadressekartoteket.</span><span class="sxs-lookup"><span data-stu-id="9d612-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="9d612-116">Se [Procedurer for offlineadressekartotek](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="9d612-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
