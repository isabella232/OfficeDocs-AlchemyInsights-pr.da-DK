---
title: 'Fejl: Reglerne på denne computer stemmer ikke overens'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782946"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="93f06-102">Fejl: Reglerne på denne computer stemmer ikke overens</span><span class="sxs-lookup"><span data-stu-id="93f06-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="93f06-103">Hvis du vil have vist opdateret status for dette kendte problem, [skal du se Reglerne på denne computer svarer ikke til reglerne i Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="93f06-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="93f06-104">Outlook-teamet har implementeret en rettelse i build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="93f06-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="93f06-105">Rettelsen er allerede i Insider Fast og går til Månedlig kanal sidst i juni 2020.</span><span class="sxs-lookup"><span data-stu-id="93f06-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="93f06-106">Når du har den rettede build, får du muligvis prompten "Hvilke regler vil du beholde" en sidste gang.</span><span class="sxs-lookup"><span data-stu-id="93f06-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="93f06-107">Vælg Server, når du bliver bedt om det, og gå derefter tilbage til Outlook og genaktiver alle regler, der blev deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="93f06-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="93f06-108">Indtil rettelsen er tilgængelig, skal du bruge følgende løsning:</span><span class="sxs-lookup"><span data-stu-id="93f06-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="93f06-109">**Løsning:** I de seneste rapporter er problemet mest forekommet hos personer, der kun har oprettet klientregler i skrivebordsversionen af Outlook.</span><span class="sxs-lookup"><span data-stu-id="93f06-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="93f06-110">Hvis du fortsat løber ind i problemet, kan du overveje at slette reglerne og derefter kun oprette og redigere regler i OWA (Outlook Web App), indtil problemet er løst.</span><span class="sxs-lookup"><span data-stu-id="93f06-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="93f06-111">Hvis du ikke kan slette reglerne manuelt, kan du køre en Outlook-kommando, når du starter Outlook, ved at køre Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="93f06-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="93f06-112">Dette sletter både klient- og serverreglerne.</span><span class="sxs-lookup"><span data-stu-id="93f06-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="93f06-113">Det sletter alle reglerne for alle konti i Outlook-profilen.</span><span class="sxs-lookup"><span data-stu-id="93f06-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="93f06-114">Denne kommando er yderligere dokumenteret i artiklen om kommandolinjeparametre.</span><span class="sxs-lookup"><span data-stu-id="93f06-114">This command is further documented in the Command-line switches article.</span></span>

