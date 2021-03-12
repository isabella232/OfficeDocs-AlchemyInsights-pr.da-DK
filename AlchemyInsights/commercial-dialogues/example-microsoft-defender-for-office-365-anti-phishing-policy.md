---
title: Eksempel på politik for microsoft defender til Office 365-antiphishing
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744894"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="ab055-102">Eksempel på politik for microsoft defender til Office 365-antiphishing</span><span class="sxs-lookup"><span data-stu-id="ab055-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="ab055-103">Disse indstillinger aktiverer en politik med navnet *Domæne og administrerende direktør.*</span><span class="sxs-lookup"><span data-stu-id="ab055-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="ab055-104">Denne politik giver både bruger- og domænebeskyttelse mod efterligning og anvender derefter politikken på alle mails, der modtages af brugere på domænet.</span><span class="sxs-lookup"><span data-stu-id="ab055-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="ab055-105">Først skal du tilføje følgende oplysninger for at oprette politikken:</span><span class="sxs-lookup"><span data-stu-id="ab055-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="ab055-106">**Navn:** Beskrivelse af domæne **og administrerende direktør:** Sikrer, at den administrerende direktør og dit domæne ikke bliver efterligning.</span><span class="sxs-lookup"><span data-stu-id="ab055-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="ab055-107">**Anvendt på:** Vælg **modtagerdomænet er.**</span><span class="sxs-lookup"><span data-stu-id="ab055-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="ab055-108">Under **En af disse** skal du **vælge** Vælg og derefter vælge et domæne.</span><span class="sxs-lookup"><span data-stu-id="ab055-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="ab055-109">Vælg **+ Tilføj.**</span><span class="sxs-lookup"><span data-stu-id="ab055-109">Select **+ Add**.</span></span> <span data-ttu-id="ab055-110">Markér afkrydsningsfeltet ud for navnet på domænet på listen (f.eks. *contoso.com),* og vælg derefter **Tilføj.**</span><span class="sxs-lookup"><span data-stu-id="ab055-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="ab055-111">Vælg **Udført.**</span><span class="sxs-lookup"><span data-stu-id="ab055-111">Select **Done**.</span></span>
- <span data-ttu-id="ab055-112">Når politikken er oprettet, kan du finjustere politikken ved hjælp af følgende indstillinger:</span><span class="sxs-lookup"><span data-stu-id="ab055-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="ab055-113">**Tilføj brugere, der skal beskyttes:** I dette eksempel skal du som minimum tilføje den administrerende direktørs mailadresse.</span><span class="sxs-lookup"><span data-stu-id="ab055-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="ab055-114">**Tilføj domæner, der skal beskyttes:** Tilføj det organisatoriske domæne, der omfatter den administrerende direktørs kontor.</span><span class="sxs-lookup"><span data-stu-id="ab055-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="ab055-115">**Vælg handlinger:** Hvis mail sendes af en efterligning af en **bruger,** skal du vælge Omdiriger meddelelse til en anden mailadresse og derefter angive mailadressen på sikkerhedsadministratoren (f.eks. *securityadmin@contoso.com).* </span><span class="sxs-lookup"><span data-stu-id="ab055-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="ab055-116">Hvis **mail sendes af et efterligningsdomæne, skal** du vælge Sæt meddelelsen i **karantæne.**</span><span class="sxs-lookup"><span data-stu-id="ab055-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="ab055-117">**Postkasseintelligens:** Denne indstilling vælges som standard, når du opretter en ny antiphishingpolitik.</span><span class="sxs-lookup"><span data-stu-id="ab055-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="ab055-118">Lad denne indstilling være tændt for **at** få de bedste resultater.</span><span class="sxs-lookup"><span data-stu-id="ab055-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="ab055-119">**Tilføj afsendere og domæner, der er tillid til:** I dette eksempel skal du ikke definere nogen tilsidesættelser.</span><span class="sxs-lookup"><span data-stu-id="ab055-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="ab055-120">Når du har gennemset dine indstillinger, skal du **vælge Opret denne politik** eller **Gem** efter behov.</span><span class="sxs-lookup"><span data-stu-id="ab055-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="ab055-121">Du kan få mere at vide [under Politikker for antiphishing i Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="ab055-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
