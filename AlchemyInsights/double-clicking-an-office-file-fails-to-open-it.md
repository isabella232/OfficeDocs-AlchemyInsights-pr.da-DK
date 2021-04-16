---
title: Når du dobbeltklikker på en Office-fil, åbnes den ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814799"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="0798b-102">Når du dobbeltklikker på en Office-fil, åbnes den ikke</span><span class="sxs-lookup"><span data-stu-id="0798b-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="0798b-103">Når du dobbeltklikker på en Office-fil, kan du se programmet åbne, men selve filen åbnes ikke.</span><span class="sxs-lookup"><span data-stu-id="0798b-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="0798b-104">Eller du får muligvis fejlen: "Der opstod et problem med at sende kommandoen til programmet."</span><span class="sxs-lookup"><span data-stu-id="0798b-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="0798b-105">Der er mange årsager til dette, men de to mest almindelige løsninger er:</span><span class="sxs-lookup"><span data-stu-id="0798b-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="0798b-106">I Excel skal du sikre dig, at DDE-indstillingen ikke er markeret.</span><span class="sxs-lookup"><span data-stu-id="0798b-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="0798b-107">Indstillingen kan findes ved at oprette en ny projektmappe og derefter vælge Filer **> Indstillinger > Avanceret**.</span><span class="sxs-lookup"><span data-stu-id="0798b-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="0798b-108">I sektionen **Generelt skal** du fjerne markeringen i **Ignorer andre programmer, der bruger Dynamic Data Exchange (DDE).**</span><span class="sxs-lookup"><span data-stu-id="0798b-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="0798b-109">Kør en onlinereparation for at gendanne standardindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="0798b-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="0798b-110">Klik på knappen Start i Windows, og søg efter "Kontrolpanel".</span><span class="sxs-lookup"><span data-stu-id="0798b-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="0798b-111">Åbn **Kontrolpanel ,** og gå til **Programmer > Programmer og funktioner**.</span><span class="sxs-lookup"><span data-stu-id="0798b-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="0798b-112">Højreklik derefter på **Microsoft Office [Version], og** vælg Skift > **Onlinereparation**.</span><span class="sxs-lookup"><span data-stu-id="0798b-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="0798b-113">Hvis ingen af disse løsninger virker, kan du finde en mere komplet liste over løsninger i supportartikel, hvor du ikke kan åbne [en Office-fil ved at dobbeltklikke på den.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="0798b-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
