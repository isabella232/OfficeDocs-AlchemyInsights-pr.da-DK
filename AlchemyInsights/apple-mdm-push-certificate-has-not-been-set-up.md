---
title: Apple MDM Push Certificate er ikke konfigureret
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
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439015"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Certificate er ikke konfigureret

Der er ikke konfigureret et Apple MDM Push-certifikat (også kaldet et APNS-certifikat (Apple Push Notification Service) til dit abonnement. Uden et Apple MDM Push-certifikat konfigureret kan du ikke tilmelde og administrere iOS- og Mac OS-enheder. Når du har tilføjet certifikatet til Intune, kan brugerne installere appen Firmaportal for at tilmelde deres iOS-enheder.

1. Vælg **"Jeg accepterer".** for at give Microsoft tilladelse til at sende data til Apple.

2. Vælg **Hent din CSR-anmodning** om at signere intune-certifikat, der kræves for at oprette et Apple MDM-pushcertifikat. Filen bruges til at anmode om et tillidsforholdscertifikat fra Apple Push-certifikatportalen.

3. Vælg **Opret dit MDM-pushcertifikat** for at gå til Apple Push Certificates Portal. Log på med dit firmas Apple-id, og vælg derefter **Opret et certifikat**. Vælg **Vælg fil ,** gå til filen med anmodning om certifikatsignering, og vælg derefter **Overfør**. På siden Bekræftelse skal du vælge **Hent** for at hente certifikatfilen (.pem) og gemme filen lokalt.
 
**Bemærk:** Certifikatet er knyttet til det Apple-id, der blev brugt til at oprette det. Som en bedste fremgangsmåde kan du bruge et apple-id til administrationsopgaver og sørge for, at postkassen overvåges af mere end én person eller ved hjælp af en distributionsliste. Brug aldrig et personligt Apple-id. Brug det samme Apple-id til at forny Apple Push-certifikatet hver 12.
 
4. Angiv det Apple-id, der bruges til at oprette dit Apple MDM-pushcertifikat. Registrer dette id som en påmindelse om, hvornår du skal forny certifikatet.

5. Gå til certifikatfilen (.pem), vælg **Åbn**, og vælg derefter **Overfør**. Med push-certifikatet kan Intune tilmelde og administrere Apple-enheder.