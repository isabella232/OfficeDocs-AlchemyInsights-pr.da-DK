---
title: Problem med sikkerhedsgrupper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177419"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="b609b-102">Problem med sikkerhedsgrupper</span><span class="sxs-lookup"><span data-stu-id="b609b-102">Issue with security groups</span></span>

<span data-ttu-id="b609b-103">**Hvis du får netværksfejlen AADDS104**</span><span class="sxs-lookup"><span data-stu-id="b609b-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="b609b-104">Ugyldige regler for netværkssikkerhedsgruppe er den mest almindelige årsag til netværksfejl i Azure Active Directory-domæneservices (AD DS).</span><span class="sxs-lookup"><span data-stu-id="b609b-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="b609b-105">Netværkssikkerhedsgruppen for det virtuelle netværk skal tillade adgang til bestemte porte og protokoller.</span><span class="sxs-lookup"><span data-stu-id="b609b-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="b609b-106">Hvis disse porte blokeres, kan Azure-platformen ikke overvåge eller opdatere det administrerede domæne.</span><span class="sxs-lookup"><span data-stu-id="b609b-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="b609b-107">Synkroniseringen mellem Azure AD og Azure AD DS påvirkes også.</span><span class="sxs-lookup"><span data-stu-id="b609b-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="b609b-108">Sørg for, at standardportene er åbne for at undgå afbrydelser af tjenesten.</span><span class="sxs-lookup"><span data-stu-id="b609b-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="b609b-109">Hvis du vil forstå og løse almindelige beskeder om konfigurationsproblemer med netværkssikkerhedsgrupper, skal du [se Tilføj og Bekræft sikkerhedsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="b609b-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
