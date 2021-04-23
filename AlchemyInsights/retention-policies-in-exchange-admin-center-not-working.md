---
title: Opbevaringspolitikker i Exchange Administration fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952222"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="3c54d-102">Opbevaringspolitikker i Exchange Administration</span><span class="sxs-lookup"><span data-stu-id="3c54d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="3c54d-103">Hvis du vil have os til at køre automatiserede kontroller af de indstillinger, der er nævnt nedenfor, skal du vælge knappen Tilbage < – øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med opbevaringspolitikkerne.</span><span class="sxs-lookup"><span data-stu-id="3c54d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="3c54d-104">Hvis du har problemer med opbevaringspolitikker i Exchange Administration, der ikke gælder for postkasser eller elementer, der ikke flyttes til arkivpostkassen, skal du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="3c54d-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="3c54d-105">**Rodårsagen:**</span><span class="sxs-lookup"><span data-stu-id="3c54d-105">**Root Causes:**</span></span>

- <span data-ttu-id="3c54d-106">**Administreret mappeassistent** har ikke behandlet brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="3c54d-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="3c54d-107">Den administrerede mappeassistent forsøger at behandle hver postkasse i din skybaserede organisation én gang hver syv dage.</span><span class="sxs-lookup"><span data-stu-id="3c54d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="3c54d-108">**Løsning:** Kør assistenten til administrerede mapper.</span><span class="sxs-lookup"><span data-stu-id="3c54d-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="3c54d-109">**Opbevaringshold** er **aktiveret** på postkassen.</span><span class="sxs-lookup"><span data-stu-id="3c54d-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="3c54d-110">Hvis postkassen er placeret på en Opbevaringshold, behandles opbevaringspolitikken for postkassen ikke i dette tidsrum.</span><span class="sxs-lookup"><span data-stu-id="3c54d-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="3c54d-111">**Løsning:** Kontrollér status for indstilling og opdatering af Opbevaringsposition efter behov.</span><span class="sxs-lookup"><span data-stu-id="3c54d-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="3c54d-112">Du kan få mere at vide under [Opbevaringsposition for postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="3c54d-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="3c54d-113">**Bemærk!** Hvis en postkasse er mindre end 10 MB, behandler den administrerede mappeassistent ikke automatisk postkassen.</span><span class="sxs-lookup"><span data-stu-id="3c54d-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="3c54d-114">Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration i:</span><span class="sxs-lookup"><span data-stu-id="3c54d-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="3c54d-115">Opbevaringstags og opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="3c54d-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="3c54d-116">[Anvend en opbevaringspolitik på postkasser eller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Tilføj [eller fjern opbevaringsmærker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="3c54d-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="3c54d-117">Sådan identificeres den type venteposition, der er sat i en postkasse</span><span class="sxs-lookup"><span data-stu-id="3c54d-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
