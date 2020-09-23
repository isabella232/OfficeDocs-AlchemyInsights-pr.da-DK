---
title: 726 blokere mail videresendelse
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219849"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="91ec2-102">Blokere eller fjerne blokeringen af videresendelse af mail</span><span class="sxs-lookup"><span data-stu-id="91ec2-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="91ec2-103">Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du se [konfigurere videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="91ec2-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="91ec2-104">På lejerniveau foretages kontrol af ekstern videresendelse ved hjælp af udgående politik om uønsket post.</span><span class="sxs-lookup"><span data-stu-id="91ec2-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="91ec2-105">Hvis den er indstillet til fra eller automatisk, kan det blokere for videresendelse af mails med "550 5.7.520 adgang nægtet, din organisation tillader ikke ekstern videresendelse".</span><span class="sxs-lookup"><span data-stu-id="91ec2-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="91ec2-106">Hvis viderestilling blev angivet til at blive blokeret, så er den fejl, brugerne får vist.</span><span class="sxs-lookup"><span data-stu-id="91ec2-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="91ec2-107">Hvis videresendelse blokeres, skal du kontrollere, at politikken er konfigureret til at aktivere ekstern Auto Forward.</span><span class="sxs-lookup"><span data-stu-id="91ec2-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="91ec2-108">Du kan kontrollere politikken for udgående spam filter fra sikkerheds-og overholdelses Center eller ved at køre kommandoen Get-HostedOutboundSpamFilterPolicy | fl-navn, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="91ec2-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="91ec2-109">Hvis du vil konfigurere blokering af viderestilling af autoforward, vil den samme kommando fortælle dig, at politiktilstanden nu.</span><span class="sxs-lookup"><span data-stu-id="91ec2-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="91ec2-110">Bemærk! det anbefales, at du holder den eksterne Auto Forward deaktiveret på standardpolitikken for udgående spam filter og kun aktiverer den for de brugere, der har brug for ekstern videresendelse, ved at oprette en brugerdefineret politik for disse brugere.</span><span class="sxs-lookup"><span data-stu-id="91ec2-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="91ec2-111">Du kan læse mere om at [konfigurere ekstern videresendelse af mail i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="91ec2-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>