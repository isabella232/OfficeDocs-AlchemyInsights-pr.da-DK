---
title: Ændring af EWS-begrænsningsindstillinger
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818030"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="4b21e-102">Ændring af EWS-begrænsningsindstillinger</span><span class="sxs-lookup"><span data-stu-id="4b21e-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="4b21e-103">Kør vores automatiserede test, som giver dig mulighed for at ændre EWS-begrænsningspolitikken, så længe overførslen varer.</span><span class="sxs-lookup"><span data-stu-id="4b21e-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="4b21e-104">Bemærk, at selv efter denne kørsel vil EWS-importerne stadig være begrænset til 150 MB pr. 5 minutter pr. postkasse; For at opnå en højere overførselshastighed, skal du overføre flere brugere samtidigt.</span><span class="sxs-lookup"><span data-stu-id="4b21e-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="4b21e-105">Bemærk, at ændringer i EWS-begrænsningspolitikken ikke har nogen indflydelse på følgende overførselstyper (ved hjælp af Microsoft-værktøjer): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Offentlig mappe eller PST-importtjeneste.</span><span class="sxs-lookup"><span data-stu-id="4b21e-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>