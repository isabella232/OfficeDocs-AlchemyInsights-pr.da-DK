---
title: Virtuel konfiguration med AAD-domæne tjenester
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884975"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="43042-102">Virtuel konfiguration med AAD-domæne tjenester</span><span class="sxs-lookup"><span data-stu-id="43042-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="43042-103">Virtuel konfiguration med AAD-domæne tjenester involverer følgende trin:</span><span class="sxs-lookup"><span data-stu-id="43042-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="43042-104">Kontrollere domænets tilstand på Azure-portalen https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="43042-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="43042-105">Kontrollér din NSG for regler, der blokerer de porte, der kræves for at synkronisere i Azure AD-domæne tjenester på portalen https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="43042-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="43042-106">Sikre, at dit virtuelle netværk er installeret i det samme Azure-område som dit Azure AD Domain Services-administreret domæne.</span><span class="sxs-lookup"><span data-stu-id="43042-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="43042-107">Sørg for, at du ikke har et eksisterende domæne med det samme domænenavn, der er tilgængeligt på det virtuelle netværk.</span><span class="sxs-lookup"><span data-stu-id="43042-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="43042-108">Du kan finde flere oplysninger om Designovervejelser i Azure virtuelt netværk, der understøtter AAD-domæne tjenester, under overvejelser i forbindelse med [virtuelt netværk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="43042-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

