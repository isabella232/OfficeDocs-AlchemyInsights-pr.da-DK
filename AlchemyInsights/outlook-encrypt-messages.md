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
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053219"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="bda7d-102">Kryptér e-mail-meddelelser i Outlook</span><span class="sxs-lookup"><span data-stu-id="bda7d-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="bda7d-103">Office 365-meddelelseskryptering er baseret på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure information Protection.</span><span class="sxs-lookup"><span data-stu-id="bda7d-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="bda7d-104">Hvis dit abonnement omfatter Azure Rights Management eller Azure information Protection, **behøver du ikke foretage dig noget for manuelt at aktivere eller aktivere** Rights Management-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="bda7d-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="bda7d-105">Baseret på kundefeedback vil vi ikke længere aktivere Exchange mail flow-regler for automatisk at kryptere udgående mails, der indeholder visse typer af følsomme oplysninger i din lejer som standard.</span><span class="sxs-lookup"><span data-stu-id="bda7d-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="bda7d-106">I stedet giver vi detaljerede instruktioner om, hvordan du kan gøre det selv.</span><span class="sxs-lookup"><span data-stu-id="bda7d-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="bda7d-107">Yderligere oplysninger om, hvordan du opretter en transportregel til kryptering af følsomme oplysninger, finder du i [denne artikel](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="bda7d-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="bda7d-108">Hvis du bruger Outlook på internettet (tidligere **OWA**): når du komponerer en e-mail-besked, skal du blot klikke på **Beskyt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="bda7d-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="bda7d-109">Dette vil gælde "Videresend ikke"-tilladelse.</span><span class="sxs-lookup"><span data-stu-id="bda7d-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="bda7d-110">Klik på **Skift tilladelse** , og vælg **Kryptér** for kun at kryptere meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="bda7d-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="bda7d-111">Hvis du **bruger Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Options** > **tilladelser**og derefter vælge den ønskede beskyttelses indstilling.</span><span class="sxs-lookup"><span data-stu-id="bda7d-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="bda7d-112">Hvis du **automatisk vil kryptere alle mails** , der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en transportregel for e-mail-strømmen i Exchange administration.</span><span class="sxs-lookup"><span data-stu-id="bda7d-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="bda7d-113">Detaljerede anvisninger er angivet i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="bda7d-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

