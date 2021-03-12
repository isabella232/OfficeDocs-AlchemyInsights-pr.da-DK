---
title: Løs almindelige problemer med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744887"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="e44fd-102">Løs almindelige problemer med DKIM-postformatering</span><span class="sxs-lookup"><span data-stu-id="e44fd-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="e44fd-103">De fleste problemer med DKIM-konfiguration er relateret til forkerte DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="e44fd-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="e44fd-104">For at løse problemer med DKIM-opsætningen skal du kontrollere, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt.</span><span class="sxs-lookup"><span data-stu-id="e44fd-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e44fd-105">Du kan finde flere oplysninger [under Hvad du skal gøre for manuelt at konfigurere DKIM i Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="e44fd-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="e44fd-106">Hvis du har brug for generel hjælp til DNS-poster, kan du se [Oprette DNS-poster for Office 365 hos](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)en hvilken som helst DNS-udbyder.</span><span class="sxs-lookup"><span data-stu-id="e44fd-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="e44fd-107">Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne, skal du vente på, at DNS-posterne bliver overført.</span><span class="sxs-lookup"><span data-stu-id="e44fd-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
