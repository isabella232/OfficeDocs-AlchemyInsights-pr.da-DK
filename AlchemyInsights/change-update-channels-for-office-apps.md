---
title: Ændre opdateringskanaler for Office-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439016"
---
# <a name="change-update-channels-for-office-apps"></a>Ændre opdateringskanaler for Office-apps

I forbindelse med nye Office-installationer skal du bruge Office Software Download Settings til at vælge den ønskede opdateringskanal og derefter installere (eller geninstallere) Office-apps. Du kan finde flere oplysninger under [Administrere indstillinger for overførsel af software i Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Bemærk:** Den opdateringskanal, der er valgt ved hjælp af Office Software Download Settings, gælder for alle brugere, der udfører nye installationer ved hjælp af O365-portalen. Du kan finde flere oplysninger [under Downloade og installere eller geninstallere Microsoft 365 eller Office 2019 på en pc eller Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

I forbindelse med eksisterende Office-installationer skal du bruge ODT (Office Deployment Tool) til at skifte til en anden opdateringskanal:  

1. Hent den nyeste version af Office Deployment Tool (setup.exe) fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identificer navnet på den kanal, du vil skifte til. Yderligere oplysninger under Konfigurationsindstillinger [for Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Opret en XML-konfigurationsfil, der angiver det relevante kanalnavn, fupdate.xml.  
    a. <Configuration>  
    b. <**opdaterer Channel="Månedligt"** />  
    c. </Configuration>
4. Fra en kommandoprompt med en høj kommando skal du skifte til den mappeplacering, setup.exe er placeret, og køre følgende kommando:  
    a. setup.exe /configure update.xml
5. Start et Office-program (f.eks. **File**  >  **Account** Vælg Opdater opdateringsindstillinger nu i **sektionen**  >  **Produktoplysninger**.

Du kan finde flere oplysninger [under Sådan skifter du opdateringskanaler til eksisterende Office-apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Hvis du vil skifte opdateringskanaler for en valgt gruppe af brugere eller ved hjælp af Configuration Manager (SCCM), skal du konfigurere indstillingen Opdater kanal ved hjælp af gruppepolitikobjekter. Du kan finde flere oplysninger [under Oversigt over opdateringskanaler til Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Du kan finde flere oplysninger [under Sådan administrerer du Office 365 ProPlus-kanaler til it-teknikere](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) [og administrerer opdateringer til Microsoft 365-apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).