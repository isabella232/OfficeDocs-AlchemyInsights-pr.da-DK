---
title: Proxyadressefejl under oprettelse af en delt postkasse
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062902"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxyadressefejl under oprettelse af en postkasse eller et andet mailaktiveret objekt

Hvis du har forsøgt at oprette et mailaktiveret objekt (postkasse, delt postkasse osv.) og får fejlmeddelelsen "Proxyadressen "SMTP:alias@domain.com" er allerede i brug...", så er den mailadresse, du har valgt, allerede taget af et andet mailaktiveret objekt i organisationen.
  
Du skal finde den bruger, gruppe, delte postkasse eller offentlige mappe, der har denne mailadresse, og slette den eller ændre dens mailadresse. Derefter kan du oprette et nyt mailaktiveret objekt med den frigjorte mailadresse. Brug Søgefunktionen på startsiden til at finde den. Du kan også bruge følgende Exchange Online PowerShell-kommando til at søge efter den:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Hvis du ikke vil slette den eksisterende mailadresse, skal du vælge en ny mailadresse til det nye objekt, du opretter.
  