---
title: Teams 4c7 fejl
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796040"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fejl i Microsoft teams

Denne fejl opstår, fordi Microsoft teams kræver formulargodkendelse. Når du implementerer Active Directory Federation Services (AD FS), er formulargodkendelse ikke aktiveret for intranettet som standard. Hvis Windows-integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.

Du kan lÃ ̧se problemet ved at aktivere formulargodkendelse ved hjÃ ¦ lp af snap-in'en AD FS Microsoft Management Console (MMC) pÃ ¥ den computer, der har den lokale kopi af Active Directory. Dette gøres ved at benytte følgende fremgangsmåde: 

1. Gå til **godkendelsespolitikker**i navigationsruden.
2. Under **handlinger** i detaljeruden skal du vælge **Rediger global primær godkendelse**.
3. Vælg **formulargodkendelse**under fanen **intranet** .
4. Vælg **OK** (eller **Anvend**).