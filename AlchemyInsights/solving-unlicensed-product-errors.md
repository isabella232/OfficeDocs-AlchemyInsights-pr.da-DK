---
title: Løsning af produktfejl uden licens
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 87a0a2be6b222d35acbc862eed4f14fb3e3e36ac
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764147"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Forslag til løsning af fejl i "Produkt uden licens"

Hvis du vil løse fejl omkring et produkt uden licens, kan du prøve følgende:

- Kontrollér, om din abonnementsstatus er udløbet.
- Sørg for, at du har et abonnement, der tillader klientlicenser, f.eks. [ensure that the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users) 
- Sørg for, at brugeren logger på Office med den samme konto, som licensen er tildelt.
- Tjek [siden Tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at se, om der er kendte problemer med tjenesten.
- Kontroller dine firewall-, antivirusprogrammers og proxyindstillinger for at bekræfte, at de ikke blokerer for, at Office-apps får adgang til internettet. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan også prøve følgende fejlfindingshandlinger: 

- Åbn en Office-app, og [log af](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brugerkonti. [Fjern](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) og [gentildel Office-licensen,](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) og log derefter [på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ved hjælp af den berørte brugerkonto.
- Kør [fejlfindingsværktøjet til aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Nulstil Aktiveringstilstanden i Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Udfør en onlinereparation af Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Hvis du vil have yderligere fejlfindingsløsninger, skal du se: 

- [Fejl i forbindelse med produkt uden licens og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)