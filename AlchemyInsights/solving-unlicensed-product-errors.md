---
title: Løsning af fejl med produkt uden licens
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786843"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Forslag til løsning af fejl med "Produkt uden licens"

Hvis du vil løse fejl i et produkt uden licens, kan du prøve følgende:

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, f.eks. Microsoft 365 Apps til virksomheder eller Business Premium, og sørg for, at brugeren har fået [tildelt en licens.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Sørg for, at brugeren logger på Office med den samme konto, som er tildelt licensen.
- Kontrollér siden [Tjenestestilstand for](https://docs.microsoft.com/office365/enterprise/view-service-health) at se, om der er kendte problemer med tjenesten.
- Kontrollér dine firewall-, antivirussoftware- og proxyindstillinger for at bekræfte, at de ikke blokerer for adgang til Microsoft 365-apps på internettet. Se [URL-adresser og IP-adresseintervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan også prøve følgende fejlfindingshandlinger: 

- Åbn en Office-app, [og log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af eventuelle eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) igen, og [log derefter på Office med](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) den pågældende brugerkonto.
- Kør [fejlfindingsværktøjet Aktivering.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Nulstil Office-aktiveringstilstanden.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state) 
- [Udfør en onlinereparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Hvis du vil have yderligere fejlfindingsløsninger, skal du se: 

- [Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)