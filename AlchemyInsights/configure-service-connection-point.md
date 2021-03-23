---
title: Konfigurere serviceforbindelsespunkt (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035449"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurere serviceforbindelsespunkt (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Årsag:** Det er ikke muligt at læse SCP-objektet og hente Azure AD-lejeroplysningerne
- **Løsning:** Se afsnittet Konfigurer [et tjenesteforbindelsespunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Handlingsplan**

- Kontrollér, om enheden har modtaget gruppepolitikobjektet for den kontrollerede validering.
- Kontrollér, at gruppepolitikobjektet har oprettet registreringsdatabasenøglerne.
- Sørg for, at du har to nøgler oprettet med dit mappe-id og dit onmicrosoft-domæne.

**Konfigurer indstilling for registreringsdatabase på klientsiden for SCP**

Brug følgende eksempel til at oprette et Gruppepolitik-objekt (GPO) til at installere en indstilling i registreringsdatabasen, der konfigurerer en SCP-post i registreringsdatabasen på dine enheder.

1. Åbn en Gruppepolitik administrationskonsol, og opret et nyt gruppepolitikobjekt i dit domæne.
     - Giv dit nyoprettede gruppepolitikobjekt et navn (f.eks. ClientSideSCP)

2. Rediger gruppepolitikobjektet, og find følgende sti: Computerkonfiguration > **Indstillinger > Windows-indstillinger > registreringsdatabase.**

3. Højreklik på **registreringsdatabasen, og** vælg **Ny > registreringsdatabaseelement.**

4. Konfigurer **følgende** under fanen Generelt:
  
- **Handling:** Opdater
    
- **Hive:** HKEY_LOCAL_MACHINE
    
- **Nøglesti:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Værdinavn:** TenantId
    
- **Værditype:** REG_SZ
    
- **Værdidata:** GUID'et eller mappe-id'et for din Azure AD-forekomst (denne værdi kan findes i **Azure-portalen > Azure Active Directory > Properties > Directory-id)**
 
- Klik på **OK**.
 
5. Højreklik på **registreringsdatabasen, og** vælg **Ny > registreringsdatabaseelement.**

6. Konfigurer **følgende** under fanen Generelt:
  
- **Handling:** Opdater
    
- **Hive:** HKEY_LOCAL_MACHINE
    
- **Nøglesti:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Værdinavn:** TenantName
    
- **Værditype:** REG_SZ
    
- **Værdidata:** Dit bekræftede domænenavn, hvis du bruger et miljø i organisationsnetværket, f.eks. AD FS. Dit bekræftede domænenavn eller dit onmicrosoft.com (f.eks. contoso.onmicrosoft).com, hvis du bruger administreret miljø

- Klik på **OK**.

7. Luk editoren for det nyoprettede gruppepolitikobjekt.

8. Sammenkæd det nyoprettede gruppepolitikobjekt med de ønskede OU'er, der indeholder domænetilføjede computere, som tilhører din kontrollerede implementerings population.

Du kan finde flere oplysninger under [Kontrolleret validering af hybrid Azure AD-joinforbindelse – Azure AD | Microsoft Docs og](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) fejlfinding [af hybridenheder, der er forbundet til Azure Active Directory, | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)









