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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473095"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="a405e-102">Blokere eller fjerne blokeringen af videresendelse af mail</span><span class="sxs-lookup"><span data-stu-id="a405e-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="a405e-103">Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du se [konfigurere videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="a405e-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="a405e-104">På lejerniveau er kontrol af ekstern videresendelse udført ved hjælp af den udgående spam politik.</span><span class="sxs-lookup"><span data-stu-id="a405e-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="a405e-105">Du kan kontrollere politikken for udgående spamfilter fra sikkerhed og overholdelses Center [her] ( https://protection.office.com/antispam) eller ved hjælp af [kommandoen Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="a405e-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="a405e-106">Hvis du får vist følgende fejlmeddelelse: **"550 5.7.520 adgang nægtet, din organisation tillader ikke ekstern videresendelse"**, skal du sørge for, at politikken er konfigureret til at aktivere ekstern automatisk videresendelse.</span><span class="sxs-lookup"><span data-stu-id="a405e-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="a405e-107">**Bemærk:** Det anbefales, at du holder den eksterne Auto Forward deaktiveret på standardpolitikken for udgående spamfilter og kun aktiverer den for de brugere, der har brug for ekstern videresendelse, ved at oprette en brugerdefineret politik for disse brugere.</span><span class="sxs-lookup"><span data-stu-id="a405e-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="a405e-108">Du kan læse mere om at [konfigurere ekstern videresendelse af mail i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="a405e-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>