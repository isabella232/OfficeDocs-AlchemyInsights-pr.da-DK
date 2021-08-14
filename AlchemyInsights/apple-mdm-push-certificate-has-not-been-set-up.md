---
title: Apple MDM-pushcertifikat er ikke konfigureret
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
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931523"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM-pushcertifikat er ikke konfigureret

Der er ikke konfigureret et Apple MDM-pushcertifikat (også kaldet et Apple Push Notification Service (APNS)-certifikat) til dit abonnement. Uden et Apple MDM-pushcertifikat er konfigureret, kan du ikke tilmelde og administrere iOS- og Mac OS-enheder. Når du har føjet certifikatet til Intune, kan brugerne installere appen Firmaportal at tilmelde deres iOS-enheder.

1. Vælg **"Jeg accepterer".** for at give Microsoft tilladelse til at sende data til Apple.

2. Vælg **Download din CSR anmodning** om signering af Intune-certifikat, der kræves for at oprette et Apple MDM-pushcertifikat. Filen bruges til at anmode om et certifikat til tillidsforholdet fra Apple Push Certificates Portal.

3. Vælg **Opret dit MDM-pushcertifikat for** at gå til Apple Push Certificates Portal. Log på med din virksomheds Apple-id, og vælg **derefter Opret et certifikat**. Vælg **Vælg fil**, gå til filen med anmodning om certifikatsignering, og vælg derefter **Upload**. På siden Bekræftelse skal du **vælge Download** for at hente certifikatfilen (.pem) og gemme filen lokalt.
 
**Bemærk!** Certifikatet er knyttet til det Apple-id, der blev brugt til at oprette det. Som bedste fremgangsmåde skal du bruge virksomhedens Apple-id til administrationsopgaver og sørge for, at postkassen overvåges af mere end én person eller ved hjælp af en distributionsliste. Brug aldrig et personligt Apple-id. Brug det samme Apple-id til at forny Apple Push Certificate hver 12. måned.
 
4. Angiv det Apple-id, der bruges til at oprette dit Apple MDM-pushcertifikat. Registrer dette id som en påmindelse om, hvornår du skal forny certifikatet.

5. Gå til certifikatfilen (.pem), vælg **Åbn**, og vælg derefter **Upload**. Med pushcertifikatet kan Intune tilmelde sig og administrere Apple-enheder.