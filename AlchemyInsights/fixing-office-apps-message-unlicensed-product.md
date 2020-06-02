---
title: Office kan ikke aktiveres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474491"
---
# <a name="unable-to-activate-office"></a>Office kan ikke aktiveres

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, [ensure the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)f.eks.
- Sørg for, at brugeren logger på Office med den samme konto som den, der har fået licensen tildelt.
- Se [siden Tjenestetilstand for Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) for at finde ud af, om der er nogen kendte problemer med tjenesten.
- Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer internetadgangen for Office-apps. Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Office 365-URL-adresser og IP-adresseintervaller").

Brug følgende fejlfindingshandlinger:

- Åbn en Office-app, og [Log ud](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) fra alle eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Fjerne") og [Tildel](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "tildele igen") Office-licensen igen, og [log på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "logge på Office") med den pågældende brugerkonto.
- Brug [Fejlfindingsværktøj til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Nulstil aktiveringstilstand for Office](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nulstil aktiveringstilstand for Office")
- [Udfør en onlinereparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Hvis du vil have yderligere fejlfindingsløsninger, skal du se:  
[Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere" vises, når du aktiverer Office]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 "Beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere" fejl, når du aktiverer Office")