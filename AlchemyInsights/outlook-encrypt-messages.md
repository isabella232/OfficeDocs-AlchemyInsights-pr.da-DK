---
title: S/MIME-i Outlook på internettet
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666834"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="46eb2-102">Kryptere e-mails i Outlook</span><span class="sxs-lookup"><span data-stu-id="46eb2-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="46eb2-103">Office 365 meddelelseskryptering er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure beskyttelse af oplysninger.</span><span class="sxs-lookup"><span data-stu-id="46eb2-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="46eb2-104">Hvis abonnementet omfatter Azure Rights Management eller Azure beskyttelse af oplysninger, **du behøver ikke at udføre handlinger manuelt aktivere eller aktivere** Rights Management-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="46eb2-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="46eb2-105">Baseret på kundefeedback, vil vi ikke længere aktivere Exchange flow postregler kryptere udgående e-mail, der indeholder visse typer følsomme oplysninger i din lejer som standard automatisk.</span><span class="sxs-lookup"><span data-stu-id="46eb2-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="46eb2-106">I stedet vores detaljerede instruktioner om, hvordan du kan gøre det vigtige.</span><span class="sxs-lookup"><span data-stu-id="46eb2-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="46eb2-107">Du kan finde yderligere oplysninger om, hvordan du opretter en regel, transport for at kryptere følsomme oplysninger [i denne artikel](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="46eb2-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="46eb2-108">Hvis du bruger Outlook på internettet (tidligere **OWA**): Når du skriver en e-mail, skal du klikke på **Beskyt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="46eb2-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="46eb2-109">Dette gælder "Do ikke fremad" tilladelse.</span><span class="sxs-lookup"><span data-stu-id="46eb2-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="46eb2-110">Klik på **Skift tilladelse** og vælge **Krypter** kun kryptere meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="46eb2-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="46eb2-111">Hvis du bruger **Outlook-klienten**: Vælg **Indstillinger**for at sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller 2016 Outlook til Mac, > **tilladelser**og derefter vælge indstillingen beskyttelse du har brug for.</span><span class="sxs-lookup"><span data-stu-id="46eb2-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="46eb2-112">Til **automatisk at kryptere alle e-mails** sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en regel for transport flow i Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="46eb2-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="46eb2-113">Der findes detaljerede anvisninger i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="46eb2-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

