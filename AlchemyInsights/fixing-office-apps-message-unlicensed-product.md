---
title: Office kan ikke aktiveres
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812566"
---
# <a name="unable-to-activate-office"></a>Office kan ikke aktiveres

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, f.eks. Office 365 Business eller Business Premium, og sørg for, at brugeren [har en tildelt licens.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)
- Sørg for, at brugeren logger på Office med den samme konto som den, der har fået licensen tildelt.
- Se [siden Tjenestetilstand for Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) for at finde ud af, om der er nogen kendte problemer med tjenesten.
- Kontrollér dine firewall-, antivirussoftware- og proxyindstillinger for at bekræfte, at de ikke blokerer adgang til Microsoft 365-apps til internettet. Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL-adresser og IP-adresseintervaller").

**Tip** På Windows-computere kan vi diagnosticere og automatisk løse forskellige almindelige office-logonproblemer for dig. Download og kør  **[Microsoft Support- og genoprettelsesassistent for](https://aka.ms/SaRA-OfficeSignInScenario)** at bruge vores automatiserede værktøj.

Brug følgende fejlfindingshandlinger:

- Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tildel](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen igen, og [log på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.
- Brug [Fejlfindingsværktøj til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Nulstil aktiveringstilstand for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nulstil Office-aktiveringstilstand")
- [Udfør en onlinereparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Hvis du vil have yderligere fejlfindingsløsninger, skal du se:  

- [Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)