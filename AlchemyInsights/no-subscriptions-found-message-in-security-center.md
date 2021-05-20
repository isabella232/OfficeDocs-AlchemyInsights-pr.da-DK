---
title: Meddelelsen Der blev ikke fundet nogen abonnementer i Sikkerhedscenter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544102"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="f5014-102">Meddelelsen Der blev ikke fundet nogen abonnementer i Sikkerhedscenter</span><span class="sxs-lookup"><span data-stu-id="f5014-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="f5014-103">Hvis du får vist meddelelsen "Ingen abonnementer fundet", mens du åbner Microsoft Defender Security Center, betyder det, at den Azure Active Directory (AAD), der bruges til at logge brugeren på portalen, ikke har en Microsoft Defender ATP-licens.</span><span class="sxs-lookup"><span data-stu-id="f5014-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="f5014-104">Licenserne Windows E5 og Office E5 er separate licenser.</span><span class="sxs-lookup"><span data-stu-id="f5014-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="f5014-105">Åbn en supportsag, hvis licensen blev købt, men ikke er blevet klargjort for denne AAD-forekomst.</span><span class="sxs-lookup"><span data-stu-id="f5014-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="f5014-106">Enten har du:</span><span class="sxs-lookup"><span data-stu-id="f5014-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="f5014-107">Et muligt problem med klargøring af licenser.</span><span class="sxs-lookup"><span data-stu-id="f5014-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="f5014-108">Du har utilsigtet klargjort licensen til en anden Microsoft AAD end den, der bruges til godkendelse i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f5014-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>