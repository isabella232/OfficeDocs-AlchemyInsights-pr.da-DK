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
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="bc078-102">Fejlfinding af problemer med SAML-signeringscertifikatet</span><span class="sxs-lookup"><span data-stu-id="bc078-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="bc078-103">Du kan løse problemet med SAML-signeringscertifikatet ved at udføre følgende anbefalede trin:</span><span class="sxs-lookup"><span data-stu-id="bc078-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="bc078-104">Når du tilføjer et virksomhedsprogram, der understøtter SSO, genererer Azure et certifikat, der kaldes [SAML-signeringscertifikatet.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="bc078-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="bc078-105">Dette certifikat har en udløbsdato på 3 år.</span><span class="sxs-lookup"><span data-stu-id="bc078-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="bc078-106">Hvis du vil ændre udløbsdatoen for dit certifikat, skal du se Tilpasse udløbsdatoen for dit sammenslutningscertifikat og [skifte det til et nyt certifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="bc078-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="bc078-107">Azure bruger dette certifikat til at signere saml-tokens, som programmet har anmodet om, og sende det til programmet for en vellykket SSO.</span><span class="sxs-lookup"><span data-stu-id="bc078-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="bc078-108">For at fuldføre dette skal du hente certifikatet fra Azure-portalen og sende det til programleverandøren for at fuldføre SSO-processen.</span><span class="sxs-lookup"><span data-stu-id="bc078-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="bc078-109">Når processen er fuldført, har dit program tillid til dette certifikat, og alle SAML-tokens, der er signeret af dette certifikat, accepteres af programmet.</span><span class="sxs-lookup"><span data-stu-id="bc078-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="bc078-110">Hvis dette certifikat udløber, skal du oprette et nyt certifikat, opdatere det til programleverandøren og derefter gøre det aktivt på Azure-siden.</span><span class="sxs-lookup"><span data-stu-id="bc078-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="bc078-111">Du kan finde flere oplysninger i [Forny et certifikat, der snart udløber.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="bc078-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="bc078-112">Hvis certifikatet udløber, blokeres brugeren ikke.</span><span class="sxs-lookup"><span data-stu-id="bc078-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="bc078-113">[Tilføj en mailadresse for meddelelser,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) der skal modtages, før det aktuelle certifikat udløber.</span><span class="sxs-lookup"><span data-stu-id="bc078-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="bc078-114">Trin 4 er et valgfrit trin.</span><span class="sxs-lookup"><span data-stu-id="bc078-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="bc078-115">Rediger et programs SAML-certifikatsigneringsindstillinger og algoritmen til signering af certifikat.</span><span class="sxs-lookup"><span data-stu-id="bc078-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="bc078-116">Du kan finde flere oplysninger i Ændre [indstillinger for signering af certifikat og signeringsalgoritme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="bc078-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

