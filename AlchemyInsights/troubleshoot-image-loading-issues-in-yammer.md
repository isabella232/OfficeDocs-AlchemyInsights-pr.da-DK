---
title: Fejlfinding på problemer med at indlæse billeder i Yammer
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
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690237"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Fejlfinding på problemer med at indlæse billeder i Yammer

Når der opstår problemer med billeder og fil-eksempler i Yammer, kan du foretage fejlfinding ved at kontrollere, om problemet opstår for alle brugere, uanset om det sker på mobilenheder, og om det kan genskabes, når den vedhæftede fil overføres.  

**Problemer med profilbilleder**  

Hvis slutbrugerne logger på Yammer via Microsoft 365, skal de ændre deres profil, herunder deres profilbillede. Hvis brugerne ikke har tilladelse til at oprette profilopdateringer, kan en administrator udføre opdateringen for brugeren. Du kan finde flere oplysninger i [få vist og opdatere din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Du kan finde oplysninger om profil redigering, herunder profilbilleder, under [ændre min Yammer-profil og-indstillinger](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Opdaterede profil fotos synkroniseres anderledes end profil attributter. Brugere skal logge på for at begynde at synkronisere deres profilbillede. Hvis du vil have oplysninger, skal du se [brugerprofilbilleder, der er opdateret fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Du kan finde oplysninger om bruger livscyklussen for Yammer under [administrere Yammer-brugere på tværs af deres livscyklus fra Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Hvis du vil have mere at vide om, hvordan profil billed synkronisering fungerer i Microsoft 365, skal du se [oplysninger om synkronisering af profilbilleder i microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Dokument eksempler og problemer med miniaturebilleder**  

Når filer eller billeder bliver sendt til Yammer, vises eksempelvisningerne muligvis ikke, fordi: 

- Filen er beskadiget og kan ikke behandles.
- Filen er ikke for nylig blevet overført til SharePoint Online, eller Yammer har ugyldige metadata for andre årsager.
- De URL-adresser, der kræves for at indlæse eksempelbillederne, blokeres.
- Visningen af filen blev fjernet af brugeren før bogføringen.
- Et tjeneste problem forhindrede, at der blev oprettet en forhåndsvisning.

**Bemærk!** Eksempler på links og filoverførsler fungerer muligvis anderledes. Links til filer på internettet eller links, der kræver yderligere godkendelse, vises muligvis ikke korrekt.

Se [Vedhæft en fil eller et billede til en Yammer-meddelelse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)for at få flere oplysninger. 