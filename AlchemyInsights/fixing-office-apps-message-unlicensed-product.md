---
title: Kan ikke aktivere Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: e052c18eae035ff05c70a223f6d8a2eab875b2c9
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236083"
---
# <a name="unable-to-activate-office"></a>Kan ikke aktivere Office

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, f. eks Office 365 Business eller Business Premium, og [Sørg for, at brugeren har fået tildelt en licens](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Sørg for, at brugeren logger på Office med den samme konto som den, der har fået licensen tildelt.
- Se [siden Tjenestetilstand for Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) for at finde ud af, om der er nogen kendte problemer med tjenesten.
- Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Microsoft 365-apps adgang til internettet. Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL-adresser og IP-adresseintervaller").

**Tip!** På Windows-computere kan vi diagnosticere og automatisk rette flere almindelige problemer med logon til Office. Hent og Kør  **[Microsoft support-og genoprettelses assistent](https://aka.ms/SaRA-OfficeSignInScenario)** for at bruge vores automatiserede værktøj.

Brug følgende fejlfindingshandlinger:

- Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tildel](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen igen, og [log på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.
- Brug [Fejlfindingsværktøj til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Nulstil aktiveringstilstand for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nulstil Office-aktiveringstilstand")
- [Udfør en onlinereparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Hvis du vil have yderligere fejlfindingsløsninger, skal du se:  

- [Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)