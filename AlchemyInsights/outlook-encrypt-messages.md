---
title: S/MIME i Outlook på internettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764866"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="8f93d-102">Kryptere mails i Outlook</span><span class="sxs-lookup"><span data-stu-id="8f93d-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="8f93d-103">Microsoft 365-meddelelseskryptering er baseret på Azure RMS (Microsoft Azure Rights Management), som er en del af Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="8f93d-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="8f93d-104">Hvis dit abonnement omfatter Azure Rights Management eller Azure Information Protection, **behøver du ikke at foretage dig noget for manuelt at aktivere eller aktivere** Rights Management Service.</span><span class="sxs-lookup"><span data-stu-id="8f93d-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="8f93d-105">Baseret på kundefeedback vil vi ikke længere gøre det muligt for Exchange mailflowregler automatisk at kryptere udgående e-mails, der indeholder bestemte typer følsomme oplysninger i din lejer som standard.</span><span class="sxs-lookup"><span data-stu-id="8f93d-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="8f93d-106">I stedet giver vi detaljerede instruktioner om, hvordan I selv kan gøre det.</span><span class="sxs-lookup"><span data-stu-id="8f93d-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="8f93d-107">Yderligere oplysninger om, hvordan du opretter en transportregel til kryptering af følsomme oplysninger, finder du i [denne artikel](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="8f93d-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="8f93d-108">Hvis du bruger Outlook på internettet (tidligere **OWA**): Når du skriver en mail, skal du blot klikke på **Beskyt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="8f93d-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="8f93d-109">Dette gælder tilladelsen "Videresend ikke".</span><span class="sxs-lookup"><span data-stu-id="8f93d-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="8f93d-110">Klik på **Skift tilladelse,** og vælg **Krypter** for kun at kryptere meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="8f93d-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="8f93d-111">Hvis du bruger **Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Tilladelser til** > **indstillinger**og derefter vælge den beskyttelsesindstilling, du har brug for.</span><span class="sxs-lookup"><span data-stu-id="8f93d-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="8f93d-112">Hvis du automatisk vil **kryptere alle mails,** der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en regel for transport af mailflow i Exchange Administration.</span><span class="sxs-lookup"><span data-stu-id="8f93d-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="8f93d-113">Detaljerede instruktioner findes i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="8f93d-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

