---
title: Løse fejl i produkt uden licens
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737947"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Forslag til løsning af fejl med "produkt uden licens"

Hvis du vil løse fejl om et produkt uden licens, skal du prøve følgende:

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, f. eks Microsoft 365-apps til virksomheder eller virksomheds præmier, og [Sørg for, at brugeren har fået tildelt en licens](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Kontrollér, at brugeren er logget på Office med den samme konto, der har licensen tildelt.
- Kontrollér [siden Tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at se, om der er kendte problemer med tjenesten.
- Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Microsoft 365-apps adgang til internettet. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan også prøve følgende fejlfindings handlinger: 

- Åbn en Office-app, og [Log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af fra eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tildel Office-](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licensen igen, og log derefter på [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.
- Kør [fejlfindingsværktøjet til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Nulstil Office-aktiveringstilstanden](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Udføre en online reparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Hvis du vil have yderligere fejlfindingsløsninger, skal du se: 

- [Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)