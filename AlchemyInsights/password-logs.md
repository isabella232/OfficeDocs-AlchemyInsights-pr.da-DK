---
title: Adgangskodelogfiler
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524119"
---
# <a name="password-logs"></a><span data-ttu-id="1f28f-102">Adgangskodelogfiler</span><span class="sxs-lookup"><span data-stu-id="1f28f-102">Password logs</span></span>

<span data-ttu-id="1f28f-103">**Jeg har problemer med at få adgang til overvågningslogfiler til nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="1f28f-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="1f28f-104">Hvis du vil foretage fejlfinding af problemer med adgang til overvågningslogfiler til nulstilling af adgangskode, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="1f28f-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="1f28f-105">Sørg for, at du er autoriseret til at få vist overvågningslogfiler.</span><span class="sxs-lookup"><span data-stu-id="1f28f-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="1f28f-106">Kun følgende roller er godkendt:</span><span class="sxs-lookup"><span data-stu-id="1f28f-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="1f28f-107">Global administrator</span><span class="sxs-lookup"><span data-stu-id="1f28f-107">Global administrator</span></span>
 - <span data-ttu-id="1f28f-108">Sikkerhedsadministrator</span><span class="sxs-lookup"><span data-stu-id="1f28f-108">Security administrator</span></span>
 - <span data-ttu-id="1f28f-109">Sikkerhedslæser</span><span class="sxs-lookup"><span data-stu-id="1f28f-109">Security reader</span></span>

<span data-ttu-id="1f28f-110">**Jeg vil se alle overvågningshændelser for nulstilling af adgangskode fra det tidspunkt, jeg oprindeligt installerede**</span><span class="sxs-lookup"><span data-stu-id="1f28f-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="1f28f-111">Op til 120.000 nulstilling af adgangskode/registreringshændelser gemmes i rapporter for de seneste 30 dage.</span><span class="sxs-lookup"><span data-stu-id="1f28f-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="1f28f-112">Denne maksimumgrænse gælder for brugergrænsefladen, når du downloader CSV-filen.</span><span class="sxs-lookup"><span data-stu-id="1f28f-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="1f28f-113">Der er 1 million begivenheder tilgængelige via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1f28f-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="1f28f-114">Du kan finde flere oplysninger i nedenstående links:</span><span class="sxs-lookup"><span data-stu-id="1f28f-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="1f28f-115">Selvbetjeningshændelser til nulstilling af adgangskode fra Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="1f28f-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="1f28f-116">Sådan downloader du hurtigt registreringshændelser for nulstilling af adgangskode med PowerShell</span><span class="sxs-lookup"><span data-stu-id="1f28f-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="1f28f-117">**Jeg vil gerne vide mere om rapporteringsfunktioner til nulstilling af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="1f28f-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="1f28f-118">Kontrollér, hvem der registrerer eller nulstiller adgangskoder med Overvågningslogfiler til nulstilling af adgangskode i Azure-portalen under **Brugere og grupper.**</span><span class="sxs-lookup"><span data-stu-id="1f28f-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="1f28f-119">Du kan finde flere oplysninger i følgende links:</span><span class="sxs-lookup"><span data-stu-id="1f28f-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="1f28f-120">Oversigt over rapporter til nulstilling af adgangskode</span><span class="sxs-lookup"><span data-stu-id="1f28f-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="1f28f-121">Sådan får du vist rapporter om nulstilling af adgangskode i Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="1f28f-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="1f28f-122">Selvbetjeningshændelser til nulstilling af adgangskode fra Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="1f28f-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="1f28f-123">Sådan downloader du hurtigt registreringshændelser for nulstilling af adgangskode med PowerShell</span><span class="sxs-lookup"><span data-stu-id="1f28f-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


