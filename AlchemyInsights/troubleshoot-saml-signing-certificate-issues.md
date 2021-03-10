---
title: Fejlfinding af problemer med SAML-signeringscertifikat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692908"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Fejlfinding af problemer med SAML-signeringscertifikatet

Du kan løse problemet med SAML-signeringscertifikatet ved at udføre følgende anbefalede trin:

1. Når du tilføjer et virksomhedsprogram, der understøtter SSO, genererer Azure et certifikat, der kaldes [SAML-signeringscertifikatet.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Dette certifikat har en udløbsdato på 3 år. Hvis du vil ændre udløbsdatoen for dit certifikat, skal du se Tilpasse udløbsdatoen for dit sammenslutningscertifikat og [skifte det til et nyt certifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure bruger dette certifikat til at signere saml-tokens, som programmet har anmodet om, og sende det til programmet for en vellykket SSO. For at fuldføre dette skal du hente certifikatet fra Azure-portalen og sende det til programleverandøren for at fuldføre SSO-processen.

Når processen er fuldført, har dit program tillid til dette certifikat, og alle SAML-tokens, der er signeret af dette certifikat, accepteres af programmet.

3. Hvis dette certifikat udløber, skal du oprette et nyt certifikat, opdatere det til programleverandøren og derefter gøre det aktivt på Azure-siden. Du kan finde flere oplysninger i [Forny et certifikat, der snart udløber.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Hvis certifikatet udløber, blokeres brugeren ikke.

4. [Tilføj en mailadresse for meddelelser,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) der skal modtages, før det aktuelle certifikat udløber.

> [!NOTE]
> Trin 4 er et valgfrit trin.

5. Rediger et programs SAML-certifikatsigneringsindstillinger og algoritmen til signering af certifikat. Du kan finde flere oplysninger i Ændre [indstillinger for signering af certifikat og signeringsalgoritme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

