---
title: Apple MDM push-certifikatet er ikke konfigureret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716851"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM push-certifikatet er ikke konfigureret

Et Apple MDM-push-certifikat (også kaldet et APNS-certifikat (Apple Push Notification Service) er ikke konfigureret til dit abonnement. Hvis du ikke har konfigureret et Apple MDM-push-certifikat, kan du ikke registrere og administrere iOS-og Mac OS-enheder. Når du har føjet certifikatet til Intune, kan brugerne installere appen firma Portal for at registrere deres iOS-enheder.

1. Vælg **"Jeg accepterer."** Hvis du vil give Microsoft tilladelse til at sende data til Apple.

2. Vælg **Download din CSR** -anmodning om signering af Intune-certifikat for at oprette et Apple-MDM-push-certifikat. Filen bruges til at anmode om et certifikat for tillidsforhold fra Apple push Certificates-portalen.

3. Vælg **Opret dit MDM-push-certifikat** for at gå til Apple push Certificates-portalen. Log på med dit firmas Apple-ID, og vælg derefter **Opret et certifikat**. Vælg **Vælg fil**, gå til filen med anmodning om certifikat signering, og vælg derefter **Overfør**. På bekræftelsessiden skal du vælge **download** for at downloade certifikatfilen (. PEM) og gemme filen lokalt.
 
**Bemærk**! certifikatet er knyttet til det Apple-id, der bruges til at oprette det. Som en bedste fremgangsmåde skal du bruge et Apple-ID for en virksomhed til administrationsopgaver og sørge for, at postkassen overvåges af mere end én person eller ved hjælp af en distributionsliste. Brug aldrig et personligt Apple-ID. Brug samme Apple-ID til at forny Apple push-certifikatet hver tolvte måned.
 
4. Angiv det Apple-ID, der bruges til at oprette dit Apple MDM push-certifikat. Registrer dette ID som en påmindelse, når du har brug for at forny certifikatet.

5. Gå til certifikatfilen (. PEM), Vælg **Åbn**, og vælg derefter **Overfør**. Med push-certifikatet kan Intune tilmelde og administrere Apple-enheder.