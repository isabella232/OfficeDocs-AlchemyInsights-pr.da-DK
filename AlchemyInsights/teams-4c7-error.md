---
title: 4c7-fejl i teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700197"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fejl i Microsoft teams

Denne fejl opstår, fordi Microsoft teams kræver formulargodkendelse. Når du installerer Active Directory Federation Services (AD FS), er formulargodkendelse som standard ikke aktiveret for intranettet. Hvis Windows-integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.

For at løse dette problem skal du aktivere formulargodkendelse ved hjælp af MMC-snap-in'en AD FS (Microsoft Management Console) på den computer, der har den lokale kopi af Active Directory. Dette gøres ved at benytte følgende fremgangsmåde: 

1. I navigationsruden skal du gå til **godkendelsespolitikker**.
2. Under **handlinger** i ruden detaljer skal du vælge **Rediger global primær godkendelse**.
3. På fanen **intranet** skal du vælge **formulargodkendelse**.
4. Vælg **OK** (eller **Anvend**).