---
title: Fejlfinding i forbindelse med indlæsning af billeder i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148195"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Fejlfinding i forbindelse med indlæsning af billeder i Yammer

Når der opstår problemer med billeder og eksempelvisninger af filer i Yammer, skal du foretage fejlfinding ved at kontrollere, om problemet opstår for alle brugere, om det opstår på mobilenheder, og om det er reproducerbart, når den vedhæftede fil overføres.  

**Problemer med profilfoto**  

Hvis slutbrugerne logger på Yammer via Microsoft 365, skal de ændre deres profil, herunder deres profilbillede. Hvis brugerne ikke har tilladelse til at foretage profilopdateringer, kan en administrator foretage opdateringen for brugeren. Du kan finde flere oplysninger under [Få vist og opdatere din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Du kan finde flere oplysninger om profilredigering, herunder profilbilleder, under [Ændre min Yammer-profil og mine indstillinger](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Opdaterede profilbilleder synkroniseres anderledes end profilattributter. Brugerne skal logge på for at starte en synkronisering af deres profilbillede. Du kan finde flere oplysninger i [brugerprofilbilleder, der er opdateret fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Du kan finde oplysninger om brugerlivscyklussen for Yammer under [Administrere Yammer-brugere i hele deres livscyklus fra Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Du kan finde flere oplysninger om, hvordan synkronisering af profilbilleder fungerer i Microsoft 365, [under Oplysninger om synkronisering af profilbilleder i Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Problemer med dokumenteksempler og miniaturebilleder**  

Når filer eller billeder sendes til Yammer, vises forhåndsvisninger muligvis ikke, fordi: 

- Filen er beskadiget og kan ikke behandles.
- Filen er ikke for nylig blevet overført til SharePoint Online, eller Yammer har ugyldige metadata af andre årsager.
- URL-adresser, der kræves til indlæsning af eksempelbillederne, blokeres.
- Fileksemplet blev fjernet af brugeren, før det blev slået op.
- Et serviceproblem forhindrede, at der blev genereret et eksempel.

**Bemærk:** Forhåndsvisninger af links og filoverførsler kan opføre sig anderledes. Links til filer på internettet eller links, der kræver yderligere godkendelse, vises muligvis ikke korrekt.

Du kan finde flere oplysninger [under Vedhæfte en fil eller et billede til en Yammer-meddelelse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 