---
title: Flere objekter har den samme mailadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724609"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="40a08-102">Flere objekter har den samme mailadresse som identitet</span><span class="sxs-lookup"><span data-stu-id="40a08-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="40a08-103">**Flere objekter**</span><span class="sxs-lookup"><span data-stu-id="40a08-103">**Multiple objects**</span></span>

<span data-ttu-id="40a08-104">En af de almindelige årsager til denne fejl er ikke muligt at omdirigere en Outlook Web Access-anmodning korrekt i en tilstedeværelse af flere objekter, der har den samme mailadresse som identitet.</span><span class="sxs-lookup"><span data-stu-id="40a08-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="40a08-105">Hvis du vil finde disse objekter, skal du køre følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="40a08-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="40a08-106">· Hent-modtager <email address></span><span class="sxs-lookup"><span data-stu-id="40a08-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="40a08-107">· Hent-bruger <email address></span><span class="sxs-lookup"><span data-stu-id="40a08-107">· Get-User <email address></span></span>

<span data-ttu-id="40a08-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="40a08-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="40a08-109">· Hent-kontakt <email address></span><span class="sxs-lookup"><span data-stu-id="40a08-109">· Get-Contact <email address></span></span>

<span data-ttu-id="40a08-110">· Get-postkassen <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="40a08-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="40a08-111">· Get-postkassen <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="40a08-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="40a08-112">· Get-postkassen <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="40a08-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="40a08-113">Du kan løse problemet ved at fjerne flere objekter med samme mail-id og sørge for, at der er et enkelt objekt med det specifikke mail-id, og at modtager typen er UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="40a08-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="40a08-114">**Den samme adresse bruges til forretnings-og forbruger postkasser**</span><span class="sxs-lookup"><span data-stu-id="40a08-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="40a08-115">En anden årsag er, når den samme adresse bruges til forretnings-og forbruger postkasser.</span><span class="sxs-lookup"><span data-stu-id="40a08-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="40a08-116">I dette tilfælde skal brugeren ændre vedkommendes primære forbruger alias, indtil Café understøtter dette scenarie.</span><span class="sxs-lookup"><span data-stu-id="40a08-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="40a08-117">Dette er en permanent fejl, der ikke forsvinder uden indgriben.</span><span class="sxs-lookup"><span data-stu-id="40a08-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="40a08-118">Hvis du vil have mere at vide, skal du se [ændre mailadressen eller telefonnummeret til din Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="40a08-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>