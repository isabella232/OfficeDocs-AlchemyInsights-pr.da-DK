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
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="bcfef-102">Apple MDM push-certifikatet er ikke konfigureret</span><span class="sxs-lookup"><span data-stu-id="bcfef-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="bcfef-103">Et Apple MDM-push-certifikat (også kaldet et APNS-certifikat (Apple Push Notification Service) er ikke konfigureret til dit abonnement.</span><span class="sxs-lookup"><span data-stu-id="bcfef-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="bcfef-104">Hvis du ikke har konfigureret et Apple MDM-push-certifikat, kan du ikke registrere og administrere iOS-og Mac OS-enheder.</span><span class="sxs-lookup"><span data-stu-id="bcfef-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="bcfef-105">Når du har føjet certifikatet til Intune, kan brugerne installere appen firma Portal for at registrere deres iOS-enheder.</span><span class="sxs-lookup"><span data-stu-id="bcfef-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="bcfef-106">Vælg **"Jeg accepterer."**</span><span class="sxs-lookup"><span data-stu-id="bcfef-106">Select **"I agree."**</span></span> <span data-ttu-id="bcfef-107">Hvis du vil give Microsoft tilladelse til at sende data til Apple.</span><span class="sxs-lookup"><span data-stu-id="bcfef-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="bcfef-108">Vælg **Download din CSR** -anmodning om signering af Intune-certifikat for at oprette et Apple-MDM-push-certifikat.</span><span class="sxs-lookup"><span data-stu-id="bcfef-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="bcfef-109">Filen bruges til at anmode om et certifikat for tillidsforhold fra Apple push Certificates-portalen.</span><span class="sxs-lookup"><span data-stu-id="bcfef-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="bcfef-110">Vælg **Opret dit MDM-push-certifikat** for at gå til Apple push Certificates-portalen.</span><span class="sxs-lookup"><span data-stu-id="bcfef-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="bcfef-111">Log på med dit firmas Apple-ID, og vælg derefter **Opret et certifikat**.</span><span class="sxs-lookup"><span data-stu-id="bcfef-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="bcfef-112">Vælg **Vælg fil**, gå til filen med anmodning om certifikat signering, og vælg derefter **Overfør**.</span><span class="sxs-lookup"><span data-stu-id="bcfef-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="bcfef-113">På bekræftelsessiden skal du vælge **download** for at downloade certifikatfilen (. PEM) og gemme filen lokalt.</span><span class="sxs-lookup"><span data-stu-id="bcfef-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="bcfef-114">**Bemærk**! certifikatet er knyttet til det Apple-id, der bruges til at oprette det.</span><span class="sxs-lookup"><span data-stu-id="bcfef-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="bcfef-115">Som en bedste fremgangsmåde skal du bruge et Apple-ID for en virksomhed til administrationsopgaver og sørge for, at postkassen overvåges af mere end én person eller ved hjælp af en distributionsliste.</span><span class="sxs-lookup"><span data-stu-id="bcfef-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="bcfef-116">Brug aldrig et personligt Apple-ID.</span><span class="sxs-lookup"><span data-stu-id="bcfef-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="bcfef-117">Brug samme Apple-ID til at forny Apple push-certifikatet hver tolvte måned.</span><span class="sxs-lookup"><span data-stu-id="bcfef-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="bcfef-118">Angiv det Apple-ID, der bruges til at oprette dit Apple MDM push-certifikat.</span><span class="sxs-lookup"><span data-stu-id="bcfef-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="bcfef-119">Registrer dette ID som en påmindelse, når du har brug for at forny certifikatet.</span><span class="sxs-lookup"><span data-stu-id="bcfef-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="bcfef-120">Gå til certifikatfilen (. PEM), Vælg **Åbn**, og vælg derefter **Overfør**.</span><span class="sxs-lookup"><span data-stu-id="bcfef-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="bcfef-121">Med push-certifikatet kan Intune tilmelde og administrere Apple-enheder.</span><span class="sxs-lookup"><span data-stu-id="bcfef-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>