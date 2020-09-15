---
title: 'Fejl: reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690957"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="f18d6-102">Fejl: reglerne på denne computer stemmer ikke overens</span><span class="sxs-lookup"><span data-stu-id="f18d6-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="f18d6-103">Hvis du vil se en opdateret status for dette kendte problem, skal du se [reglerne på denne computer stemmer ikke overens med reglerne på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="f18d6-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="f18d6-104">Outlook-teamet har implementeret en rettelse i Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="f18d6-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="f18d6-105">Rettelsen er allerede i insider fast og vil gå til månedlig kanal i den sene juni 2020.</span><span class="sxs-lookup"><span data-stu-id="f18d6-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="f18d6-106">Når du har den faste build, kan du få meddelelsen "hvilke regler vil du gemme" en sidste gang.</span><span class="sxs-lookup"><span data-stu-id="f18d6-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="f18d6-107">Vælg server, når du bliver bedt om det, og gå derefter tilbage til Outlook, og Aktivér eventuelle regler, der er deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="f18d6-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="f18d6-108">Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:</span><span class="sxs-lookup"><span data-stu-id="f18d6-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="f18d6-109">**Løsning**: der er opstået et problem i de seneste rapporter for de personer, der kun har oprettet klientregler i Outlook på computeren.</span><span class="sxs-lookup"><span data-stu-id="f18d6-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="f18d6-110">Hvis du fortsat kører i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.</span><span class="sxs-lookup"><span data-stu-id="f18d6-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="f18d6-111">Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook ved at køre Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="f18d6-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="f18d6-112">Dette vil slette både klient-og server reglerne.</span><span class="sxs-lookup"><span data-stu-id="f18d6-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="f18d6-113">Den vil slette alle reglerne for alle konti i Outlook-profilen.</span><span class="sxs-lookup"><span data-stu-id="f18d6-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="f18d6-114">Denne kommando er yderligere dokumenteret i artiklen kommandolinjeparametre.</span><span class="sxs-lookup"><span data-stu-id="f18d6-114">This command is further documented in the Command-line switches article.</span></span>

