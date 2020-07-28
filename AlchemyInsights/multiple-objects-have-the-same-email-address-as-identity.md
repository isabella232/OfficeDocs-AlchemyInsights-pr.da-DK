---
title: Flere objekter har samme mailadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438933"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="a3030-102">Flere objekter har samme mailadresse som identitet</span><span class="sxs-lookup"><span data-stu-id="a3030-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="a3030-103">**Flere objekter**</span><span class="sxs-lookup"><span data-stu-id="a3030-103">**Multiple objects**</span></span>

<span data-ttu-id="a3030-104">En af de almindelige årsager til denne fejl er ikke at kunne distribuere en Outlook Web Access-anmodning korrekt i nærheden af flere objekter med samme mailadresse som identitet.</span><span class="sxs-lookup"><span data-stu-id="a3030-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="a3030-105">Hvis du vil finde disse objekter, skal du køre følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="a3030-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="a3030-106">· Hent modtager<email address></span><span class="sxs-lookup"><span data-stu-id="a3030-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="a3030-107">· Hent bruger<email address></span><span class="sxs-lookup"><span data-stu-id="a3030-107">· Get-User <email address></span></span>

<span data-ttu-id="a3030-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="a3030-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="a3030-109">· Get-Kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="a3030-109">· Get-Contact <email address></span></span>

<span data-ttu-id="a3030-110">· Hent postkasse <email address> -Offentligfolder</span><span class="sxs-lookup"><span data-stu-id="a3030-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="a3030-111">· Hent postkasse <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="a3030-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="a3030-112">· Hent postkasse <email address> -InaktivMailboxKun</span><span class="sxs-lookup"><span data-stu-id="a3030-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="a3030-113">Du kan løse problemet ved at fjerne flere objekter med den samme mailidentitet og sørge for, at der er et enkelt objekt med den specifikke e-mail-identitet, og at modtagertypen er UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="a3030-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="a3030-114">**Samme adresse bruges til virksomheds- og forbrugerpostkasser**</span><span class="sxs-lookup"><span data-stu-id="a3030-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="a3030-115">En anden årsag er, når den samme adresse bruges til virksomheds- og forbrugerpostkasser.</span><span class="sxs-lookup"><span data-stu-id="a3030-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="a3030-116">I dette tilfælde skal brugeren ændre sit primære forbrugeralias, indtil Cafe understøtter dette scenarie.</span><span class="sxs-lookup"><span data-stu-id="a3030-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="a3030-117">Dette er en permanent fejl, der ikke går væk uden indgriben.</span><span class="sxs-lookup"><span data-stu-id="a3030-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="a3030-118">Du kan finde flere oplysninger [under Ændre mailadressen eller telefonnummeret til din Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="a3030-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>