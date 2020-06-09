---
title: 'Fejl: Reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664240"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="628ad-102">Fejl: Reglerne på denne computer stemmer ikke overens</span><span class="sxs-lookup"><span data-stu-id="628ad-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="628ad-103">Hvis du vil se den opdaterede status for dette kendte problem, skal du se [Reglerne på denne computer stemmer ikke overens med reglerne på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="628ad-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="628ad-104">Outlook Team har implementeret en rettelse i Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="628ad-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="628ad-105">Rettelsen er allerede på Insider Fast og vil gå til Månedlig Channel i slutningen af juni 2020.</span><span class="sxs-lookup"><span data-stu-id="628ad-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="628ad-106">Når du har den faste bygge du kan få prompten "Hvilke regler vil du beholde" en sidste gang.</span><span class="sxs-lookup"><span data-stu-id="628ad-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="628ad-107">Vælg Server, når du bliver bedt om det, og gå derefter tilbage i Outlook, og genaktiver eventuelle regler, der er deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="628ad-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="628ad-108">Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:</span><span class="sxs-lookup"><span data-stu-id="628ad-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="628ad-109">**Løsning**: I de seneste rapporter er der opstået et problem for dem, der kun har oprettet klientregler i Outlook på computeren.</span><span class="sxs-lookup"><span data-stu-id="628ad-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="628ad-110">Hvis du fortsætter med at løbe ind i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.</span><span class="sxs-lookup"><span data-stu-id="628ad-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="628ad-111">Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook, ved at køre Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="628ad-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="628ad-112">Dette sletter både klient- og serverreglerne.</span><span class="sxs-lookup"><span data-stu-id="628ad-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="628ad-113">Det vil slette alle reglerne for alle konti i Outlook-profilen.</span><span class="sxs-lookup"><span data-stu-id="628ad-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="628ad-114">Denne kommando er yderligere dokumenteret i artiklen kommandolinjeparametre.</span><span class="sxs-lookup"><span data-stu-id="628ad-114">This command is further documented in the Command-line switches article.</span></span>

