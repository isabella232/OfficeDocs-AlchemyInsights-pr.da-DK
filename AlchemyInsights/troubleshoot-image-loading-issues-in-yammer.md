---
title: Fejlfinding af problemer med billedindlæsning i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939229"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Fejlfinding af problemer med billedindlæsning i Yammer

Når der opstår problemer med eksempelvisning af fotos og filer i Yammer, skal du foretage fejlfinding ved at kontrollere, om problemet opstår for alle brugere, om det sker på mobilenheder, og om det kan overføres, når du uploader den vedhæftede fil.  

**Problemer med profilbillede**  

Hvis slutbrugere logger på Yammer via Microsoft 365, skal de ændre deres profil, herunder deres profilbillede. Hvis brugerne ikke har tilladelse til at foretage profilopdateringer, kan en administrator foretage opdateringen for brugeren. Du kan få mere at [vide under Få vist og opdater din profil Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Hvis du vil have oplysninger om profilredigering, herunder profilbilleder, [skal du se Yammer profil og indstillinger](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Opdaterede profilbilleder synkroniseres anderledes end profilattributter. Brugere skal logge på for at starte en synkronisering af deres profilbillede. Du kan finde flere oplysninger [under Er brugerprofilbilleder opdateret fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Du kan finde oplysninger om brugerlivscyklussen for Yammer i [Administrere Yammer brugere på tværs](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)af deres livscyklus fra Office 365 .  

Hvis du vil have mere at vide om, hvordan synkronisering af profilbillede Microsoft 365, skal du se Oplysninger [om synkronisering af profilbillede Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Eksempler på dokumenter og problemer med billedminiaturer**  

Når filer eller billeder offentliggøres på Yammer, vises eksemplerne muligvis ikke, fordi: 

- Filen er beskadiget og kan ikke behandles.
- Filen er ikke blevet overført for nylig til SharePoint Online, eller Yammer indeholder ugyldige metadata af andre årsager.
- URL-adresser, der kræves til at indlæse eksempelbillederne, blokeres.
- Forhåndsvisningen af filen blev fjernet af brugeren, før den blev udgivet.
- Et tjenesteproblem forhindrede en forhåndsvisning i at blive genereret.

**Bemærk!** Eksempelvisninger af links og filuploads fungerer muligvis anderledes. Links til filer på internettet eller links, der kræver yderligere godkendelse, vises muligvis ikke korrekt.

Du kan få mere at vide [under Vedhæft en fil eller et billede Yammer meddelelse.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf) 