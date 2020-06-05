---
title: Oprette AIP-etiketpolitikker
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569032"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="55fcb-102">Oprette AIP-etiketpolitikker</span><span class="sxs-lookup"><span data-stu-id="55fcb-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="55fcb-103">Azure Information Protection(AIP) etiketter kan bruges sammen med hele spektret af data, som en organisation typisk opretter og gemmer, fra den laveste klassificering af personlige data, til den højeste klassificering af meget fortrolige data.</span><span class="sxs-lookup"><span data-stu-id="55fcb-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="55fcb-104">Azure Information Protection Policies gælder for den klassiske Azure Information Protection(AIP)-klient og ikke [for AIP Unified Labeling-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="55fcb-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="55fcb-105">Du kan konfigurere flere elementer i en AIP-politik, herunder indstillinger som f.eks.:</span><span class="sxs-lookup"><span data-stu-id="55fcb-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="55fcb-106">Mulighed for, hvilken etiket der vil lade administratorer eller bruger klassificere og beskytte (valgfri) dokumenter og e-mails</span><span class="sxs-lookup"><span data-stu-id="55fcb-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="55fcb-107">Mulighed for at gennemtvinge klassificering, når brugerne gemmer dokumenter og sender e-mail</span><span class="sxs-lookup"><span data-stu-id="55fcb-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="55fcb-108">Mulighed for automatisk at mærke en mail baseret på dens vedhæftede filer.</span><span class="sxs-lookup"><span data-stu-id="55fcb-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="55fcb-109">Mulighed for at styre, om blokeringslinjen til beskyttelse af oplysninger vises i Office-programmer</span><span class="sxs-lookup"><span data-stu-id="55fcb-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="55fcb-110">Du kan finde flere indstillinger og oplysninger om Azure Information Protection-politikker [under: Oversigt over politikken for Beskyttelse af Azure Information](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="55fcb-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="55fcb-111">Du kan finde andre nyttige ressourcer vedrørende AIP-politikker under:</span><span class="sxs-lookup"><span data-stu-id="55fcb-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="55fcb-112">Selvstudium: Konfigurere politikindstillinger for Azure Information Protection og oprette en ny etiket</span><span class="sxs-lookup"><span data-stu-id="55fcb-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="55fcb-113">Konfigurere politikken til beskyttelse af Azure-oplysninger</span><span class="sxs-lookup"><span data-stu-id="55fcb-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="55fcb-114">Oprette og konfigurere følsomhedsetiketter og deres politikker</span><span class="sxs-lookup"><span data-stu-id="55fcb-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="55fcb-115">Vejledninger til almindelige scenarier, der bruger Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="55fcb-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="55fcb-116">Gennemse dokumentationen til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="55fcb-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="55fcb-117">Krav til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="55fcb-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="55fcb-118">Selvstudium til hurtig start til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="55fcb-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="55fcb-119">Download Azure Information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="55fcb-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)