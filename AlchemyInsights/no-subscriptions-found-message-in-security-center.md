---
title: Meddelelse om ingen abonnementer fundet i Sikkerhedscenter
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713413"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="93e43-102">Meddelelse om ingen abonnementer fundet i Sikkerhedscenter</span><span class="sxs-lookup"><span data-stu-id="93e43-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="93e43-103">Hvis du får vist meddelelsen "Der blev ikke fundet nogen abonnementer", mens du åbner Microsoft Defender Security Center, betyder det, at det Azure Active Directory (AAD), der bruges til at logge brugeren på portalen, ikke har en Microsoft Defender ATP-licens.</span><span class="sxs-lookup"><span data-stu-id="93e43-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="93e43-104">Licenserne til Windows E5 og Office E5 er separate licenser.</span><span class="sxs-lookup"><span data-stu-id="93e43-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="93e43-105">Åbn en supportsag, hvis licensen blev købt, men ikke er klargjort til denne AAD-forekomst.</span><span class="sxs-lookup"><span data-stu-id="93e43-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="93e43-106">Enten har du:</span><span class="sxs-lookup"><span data-stu-id="93e43-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="93e43-107">Et muligt problem med klargøring af licenser.</span><span class="sxs-lookup"><span data-stu-id="93e43-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="93e43-108">Du har utilsigtet klargjort licensen til en anden Microsoft AAD end den, der blev brugt til godkendelse i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="93e43-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>