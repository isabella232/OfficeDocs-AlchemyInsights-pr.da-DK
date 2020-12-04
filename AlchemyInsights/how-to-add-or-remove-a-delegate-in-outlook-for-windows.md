---
title: Sådan tilføjer eller fjerner du en stedfortræder i Outlook til Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573339"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="89c9d-102">Sådan tilføjer eller fjerner du en stedfortræder i Outlook til Windows</span><span class="sxs-lookup"><span data-stu-id="89c9d-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="89c9d-103">Sådan tilføjer du en stedfortræder i Outlook til Windows:</span><span class="sxs-lookup"><span data-stu-id="89c9d-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="89c9d-104">Klik på fanen **filer** efterfulgt af **kontoindstillinger**, og vælg derefter **stedfortræderadgang**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="89c9d-105">Klik på **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-105">Click on **Add**.</span></span> <span data-ttu-id="89c9d-106">Hvis **Tilføj** ikke vises, findes der muligvis ikke en aktiv forbindelse mellem Outlook og Exchange.</span><span class="sxs-lookup"><span data-stu-id="89c9d-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="89c9d-107">Statuslinjen i Outlook viser Forbindelsesstatus.</span><span class="sxs-lookup"><span data-stu-id="89c9d-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="89c9d-108">Skriv navnet på den person, du vil angive som stedfortræder, eller Søg, og vælg navnet på listen over søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="89c9d-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="89c9d-109">Stedfortræderen skal være en person på din organisations globale Exchange-adresseliste (GAL).</span><span class="sxs-lookup"><span data-stu-id="89c9d-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="89c9d-110">Klik på **Tilføj** efterfulgt af **OK**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="89c9d-111">I dialogboksen **stedfortrædertilladelser** skal du acceptere standardindstillingerne for tilladelser eller vælge brugerdefinerede adgangsniveauer for Exchange-mapper.</span><span class="sxs-lookup"><span data-stu-id="89c9d-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="89c9d-112">Hvis en stedfortræder skal have tilladelse til kun at fungere med mødeindkaldelser og svar, er standardindstillingerne for tilladelse som **stedfortræder modtager kopier af møderelaterede meddelelser, der er sendt til mig** , der er tilstrækkelige.</span><span class="sxs-lookup"><span data-stu-id="89c9d-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="89c9d-113">Du kan lade **indbakkens** tilladelsesindstilling være **none**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="89c9d-114">Mødeindkaldelser og svar sendes direkte til stedfortræderens indbakke.</span><span class="sxs-lookup"><span data-stu-id="89c9d-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="89c9d-115">Som standard er stedfortræderen tildelt **redaktør (kan læse, oprette og ændre elementer)** til din **kalender** mappe.</span><span class="sxs-lookup"><span data-stu-id="89c9d-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="89c9d-116">Når stedfortræderen svarer på et møde på dine vegne, føjes det automatisk til din **kalender** mappe.</span><span class="sxs-lookup"><span data-stu-id="89c9d-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="89c9d-117">Hvis du vil sende en meddelelse for at underrette stedfortræderen om de ændrede tilladelser, skal du markere afkrydsningsfeltet **Send automatisk en meddelelse til stedfortrædere med en sammenfatning af disse tilladelser** .</span><span class="sxs-lookup"><span data-stu-id="89c9d-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="89c9d-118">Hvis du vil, kan du markere afkrydsningsfeltet **stedfortræderen kan se mine private elementer** .</span><span class="sxs-lookup"><span data-stu-id="89c9d-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="89c9d-119">Denne indstilling påvirker alle Exchange-mapper.</span><span class="sxs-lookup"><span data-stu-id="89c9d-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="89c9d-120">Dette omfatter alle mail-, kontakt-, kalender-, opgaver, noter og Journal-mapper.</span><span class="sxs-lookup"><span data-stu-id="89c9d-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="89c9d-121">Det er ikke muligt at give adgang til private elementer i bestemte mapper.</span><span class="sxs-lookup"><span data-stu-id="89c9d-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="89c9d-122">Vælg **OK**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="89c9d-123">Meddelelser, der sendes med tilladelsen Send på vegne af, omfatter både stedfortræderens og dine navne ud for **fra**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="89c9d-124">Når en meddelelse sendes med Send som-tilladelser, vises kun dit navn.</span><span class="sxs-lookup"><span data-stu-id="89c9d-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="89c9d-125">Når du har tilføjet en person som stedfortræder, kan vedkommende tilføje din Exchange-postkasse til sin Outlook-profil.</span><span class="sxs-lookup"><span data-stu-id="89c9d-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="89c9d-126">Hvis du vil have mere at vide, skal du se [administrere en anden persons mail og kalender](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="89c9d-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="89c9d-127">Sådan fjerner du en stedfortræder i Outlook til Windows:</span><span class="sxs-lookup"><span data-stu-id="89c9d-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="89c9d-128">Klik på fanen **filer** .</span><span class="sxs-lookup"><span data-stu-id="89c9d-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="89c9d-129">Klik på **kontoindstillinger** efterfulgt af **stedfortræderadgang**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="89c9d-130">Vælg navnet på den stedfortræder, du vil ændre tilladelser for, og klik derefter på **Fjern** efterfulgt af **OK**.</span><span class="sxs-lookup"><span data-stu-id="89c9d-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
