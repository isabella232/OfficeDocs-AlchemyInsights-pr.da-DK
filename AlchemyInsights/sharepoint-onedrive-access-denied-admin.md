---
title: Fejlfinding i forbindelse med meddelelser adgang nægtet
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716641"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding i forbindelse med adgang nægtet meddelelser i Sharepoint/OneDrive Admin Center

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Hvis du modtager en adgang nægtet vises, når du forsøger at gå til administrationssiden for en Sharepoint/OneDrive, skal du kontrollere, at du <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">tildeler en licens til brugeren </a>. Hvis brugeren har en licens, skal du også sikre dig de er <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">tildelt en administratorrolle</a> , der kan få adgang til admin centrum.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN). Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU). Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Du kan løse dette problem, skal du gendanne den oprindelige UPN med trinnene i artiklen, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">gendanne en bruger i Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Bemærk:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">Hvis en OneDrive eller SharePoint Administration center ikke er tilgængelig for flere brugere, som tidligere har haft adgang, kan der være et problem med den midlertidige tjeneste.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Kontrollere service sundhed dashboardet</span></a>.</span></em></span></span></p>


