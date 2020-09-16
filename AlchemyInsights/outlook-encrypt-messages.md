---
title: S/MIME i Outlook på internettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772256"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="ccfd4-102">Krypter mails i Outlook</span><span class="sxs-lookup"><span data-stu-id="ccfd4-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="ccfd4-103">Microsoft 365-meddelelseskryptering er baseret på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure information Protection.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="ccfd4-104">Hvis dit abonnement omfatter Azure Rights Management eller Azure information Protection, behøver **du ikke at foretage nogen handlinger for at aktivere eller aktivere** tjenesten Rights Management manuelt.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="ccfd4-105">Baseret på kundefeedback kan vi ikke længere aktivere regler for Exchange-mail flow for automatisk at kryptere udgående mails, der indeholder bestemte typer følsomme oplysninger i din lejer som standard.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="ccfd4-106">I stedet giver vi detaljerede anvisninger til, hvordan du kan gøre det selv.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="ccfd4-107">Du kan finde flere oplysninger om, hvordan du opretter en transportregel for at kryptere følsomme oplysninger, i [denne artikel](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="ccfd4-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="ccfd4-108">Hvis du bruger Outlook på internettet (tidligere **OWA**): når du skriver en mail, skal du blot klikke på **Beskyt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="ccfd4-109">Dette vil anvende tilladelsen "Videresend ikke".</span><span class="sxs-lookup"><span data-stu-id="ccfd4-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="ccfd4-110">Klik på **Rediger tilladelse** , og vælg **Krypter** for kun at kryptere meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="ccfd4-111">Hvis du bruger **Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Indstillinger for**  >  **tilladelser**og derefter vælge den beskyttelses indstilling, du har brug for.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="ccfd4-112">Hvis du **automatisk vil kryptere alle mails** , der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en transportregel for forsendelses strømmen i Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="ccfd4-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="ccfd4-113">Der findes detaljerede instruktioner i [denne supportartikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="ccfd4-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

