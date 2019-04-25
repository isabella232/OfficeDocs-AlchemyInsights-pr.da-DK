---
title: 1049 antiSpam 4.5.3 for mange modtagere (AS780090)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1049
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: 5bb496363b9612427e5b704cdba12b8913676885
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32397254"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="973f5-102">4.5.3 for mange modtagere (AS780090)</span><span class="sxs-lookup"><span data-stu-id="973f5-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="973f5-103">Denne fejl opstår, når e-mail-trafik fra IP-kildeadresse, overstiger den grænse, der er baseret på omdømme (eller mangel på omdømme) af kildens IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="973f5-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="973f5-104">Blokere e-mail fra kildens IP-adresse udløber inden for en time.</span><span class="sxs-lookup"><span data-stu-id="973f5-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="973f5-105">Hvis kilde-IP-adresse er en lokal e-mail-server, der tilhører dig, kan du kontrollere konfigurationen af flow mail connector.</span><span class="sxs-lookup"><span data-stu-id="973f5-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="973f5-106">Hvis problemet fortsætter i mere end en time, kan du kontakte support for at anmode om en undtagelse for kilde-IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="973f5-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
