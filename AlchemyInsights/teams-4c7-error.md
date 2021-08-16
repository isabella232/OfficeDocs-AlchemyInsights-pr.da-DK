---
title: Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049302"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fejl i Microsoft Teams

Denne fejl opstår, fordi Microsoft Teams kræver formulargodkendelse. Når du installerer Active Directory Federation Services (AD FS), er formulargodkendelse ikke aktiveret på intranettet som standard. Hvis Windows integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.

Du kan løse dette problem ved at aktivere formulargodkendelse ved hjælp af AD FS Microsoft Management Console-snap-in'en (MMC) på den computer, der har den lokale kopi af Active Directory. Dette gøres ved at benytte følgende fremgangsmåde: 

1. I navigationsruden skal du gå til **Godkendelsespolitikker**.
2. Under **Handlinger** i detaljeruden skal du vælge **Rediger global primær godkendelse.**
3. På fanen **Intranet** skal du vælge **Formulargodkendelse**.
4. Vælg **OK** (eller **Anvend).**