---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767170"
---
# <a name="troubleshoot-password-synchronization"></a>Fejlfinding i forbindelse med synkronisering af adgangskoder

Fejlfinding af problemer, hvor ingen adgangskoder er synkroniseret med Azure AD Connect version 1.1.614.0 eller nyere:
  
1. Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren med indstillingen **Kør som Administrator** . 
    
2. Køre **Set-Udførselspolitikken RemoteSigned** eller **ubegrænset sæt Udførselspolitikken**. 
    
3. Start guiden Opret forbindelse Azure AD.
    
4. Naviger til den ** yderligere opgaver ** side, Vælg ** fejlfinding **, og klik på **Næste**. 
    
5. Klik på menuen **Start til at starte fejlfindingen** PowerShell på siden fejlfinding. 
    
6. I hovedmenuen, Vælg **Fejlfinding i forbindelse med synkronisering af adgangskoder**. 
    
7. Vælg i menuen sub **adgangskodesynkronisering virker ikke på alle**. 
    
 **Forstå resultaterne af fejlfinding i forbindelse med opgaven**
  
Fejlfinding i forbindelse med opgaven udføres følgende kontrol:
  
- Validerer, at funktionen til synkronisering af adgangskode er aktiveret for din Azure AD lejer.
    
- Validerer, Azure AD Connect-serveren ikke er i midlertidig tilstand.
    
- For hver eksisterende lokale Active Directory connector (hvilket svarer til en eksisterende Active Directory-skov):
    
- 
  - Validerer, at funktionen til synkronisering af adgangskode er aktiveret.
    
  - Søger efter adgangskode synkronisering heartbeat-hændelser i logfilerne Windows Application Event.
    
  - For hver Active Directory-domæne i det lokale Active Directory connector:
    
  - Validerer, at domænet kan nås fra Azure AD Connect-serveren.
    
  - Validerer, at kontiene Active Directory-domæneservices (AD DS), der bruges af den lokale Active Directory connector har det rigtige brugernavn, adgangskode og tilladelser, der kræves af synkronisering af adgangskoder.
    
Du kan finde yderligere hjælp til fejlfinding af synkronisering af adgangskode, [fejlfinding i forbindelse med synkronisering af adgangskoder med Azure Connect for AD-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

