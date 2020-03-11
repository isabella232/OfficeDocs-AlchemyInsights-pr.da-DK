---
title: Hvis du dobbeltklikker på en Office-fil, kan den ikke åbnes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573482"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="ef84f-102">Hvis du dobbeltklikker på en Office-fil, kan den ikke åbnes</span><span class="sxs-lookup"><span data-stu-id="ef84f-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="ef84f-103">Når du har dobbeltklikket på en Office-fil, kan du muligvis se, at programmet er åbent, men selve filen åbnes ikke.</span><span class="sxs-lookup"><span data-stu-id="ef84f-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="ef84f-104">Eller du kan få fejlen: "Der opstod et problem under at sende kommandoen til programmet."</span><span class="sxs-lookup"><span data-stu-id="ef84f-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="ef84f-105">Der er mange årsager til dette, men de to mest almindelige løsninger er:</span><span class="sxs-lookup"><span data-stu-id="ef84f-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="ef84f-106">Fra Excel skal du sikre dig, at Indstillingen DDE ikke er markeret.</span><span class="sxs-lookup"><span data-stu-id="ef84f-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="ef84f-107">Indstillingen kan findes ved at oprette en ny projektmappe og derefter vælge **Fil > Indstillinger > Avanceret**.</span><span class="sxs-lookup"><span data-stu-id="ef84f-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="ef84f-108">Fjern markeringen i afkrydsningsfeltet **Ignorer andre programmer, der bruger DDE (Dynamic Data Exchange)** i sektionen **Generelt.**</span><span class="sxs-lookup"><span data-stu-id="ef84f-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="ef84f-109">Kør en onlinereparation for at gendanne standardindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="ef84f-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="ef84f-110">Klik på knappen Start i Windows, og søg efter "Kontrolpanel".</span><span class="sxs-lookup"><span data-stu-id="ef84f-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="ef84f-111">Åbn **Kontrolpanel**, og gå til **Programmer > Programmer og funktioner**.</span><span class="sxs-lookup"><span data-stu-id="ef84f-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="ef84f-112">Højreklik derefter på **Microsoft Office [Version],** og vælg **Skift > Onlinerepair**.</span><span class="sxs-lookup"><span data-stu-id="ef84f-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="ef84f-113">Hvis ingen af disse løsninger fungerer, findes der en mere komplet liste over løsninger i supportartiklen, [dobbeltklik på en Office-fil kan ikke åbneden](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="ef84f-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
