---
title: Problem med at deltage i VM'er
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884980"
---
# <a name="issue-joining-vms"></a>Problem med at deltage i VM'er

Hvis du vil løse problemer, der opstår, når du forsøger at deltage i VM'er, skal du udføre følgende trin:

1. Prøv at logge på ved hjælp af **UPN** -formatet (f. eks. ' joeuser@contoso.com ') i stedet for **sAMAccountName** -formatet (' CONTOSO\joeuser ').
2. Kontrollér, at du har aktiveret synkronisering af adgangskoder i overensstemmelse med de trin, der er angivet i *introduktions* vejledning.
3. Kontrollér, at den pågældende brugerkonto ikke er en ekstern konto i Azure AD-lejeren. Eksterne brugere kan ikke logge på det administrerede domæne, da Azure AD-domæne tjenester ikke har legitimationsoplysninger for sådanne brugerkonti.
4. Hvis den pågældende brugerkonto er en skybaseret brugerkonto, skal du sørge for, at brugerne har ændret deres adgangskode, efter du har aktiveret Azure AD-domæne tjenester. Dette trin medfører, at legitimationsoplysningerne for legitimationsoplysninger, der kræves for Azure AD-domæne tjenester oprettes.
5. Hvis de berørte brugerkonti synkroniseres fra en lokal adresseliste, skal du kontrollere, at den anbefalede version af Azure AD Connect er konfigureret til at udføre en fuld synkronisering.
6. Hvis problemet fortsætter, efter du har bekræftet trin 4, skal du udføre følgende kommandoer fra din synkroniserings maskine:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.