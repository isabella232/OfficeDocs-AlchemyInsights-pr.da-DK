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
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="6b7e6-102">Apple MDM Push Certificate er ikke konfigureret</span><span class="sxs-lookup"><span data-stu-id="6b7e6-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="6b7e6-103">Der er ikke konfigureret et Apple MDM Push-certifikat (også kaldet et APNS-certifikat (Apple Push Notification Service) til dit abonnement.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="6b7e6-104">Uden et Apple MDM Push-certifikat konfigureret kan du ikke tilmelde og administrere iOS- og Mac OS-enheder.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="6b7e6-105">Når du har tilføjet certifikatet til Intune, kan brugerne installere appen Firmaportal for at tilmelde deres iOS-enheder.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="6b7e6-106">Vælg **"Jeg accepterer".**</span><span class="sxs-lookup"><span data-stu-id="6b7e6-106">Select **"I agree."**</span></span> <span data-ttu-id="6b7e6-107">for at give Microsoft tilladelse til at sende data til Apple.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="6b7e6-108">Vælg **Hent din CSR-anmodning** om at signere intune-certifikat, der kræves for at oprette et Apple MDM-pushcertifikat.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="6b7e6-109">Filen bruges til at anmode om et tillidsforholdscertifikat fra Apple Push-certifikatportalen.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="6b7e6-110">Vælg **Opret dit MDM-pushcertifikat** for at gå til Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="6b7e6-111">Log på med dit firmas Apple-id, og vælg derefter **Opret et certifikat**.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="6b7e6-112">Vælg **Vælg fil ,** gå til filen med anmodning om certifikatsignering, og vælg derefter **Overfør**.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="6b7e6-113">På siden Bekræftelse skal du vælge **Hent** for at hente certifikatfilen (.pem) og gemme filen lokalt.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="6b7e6-114">**Bemærk:** Certifikatet er knyttet til det Apple-id, der blev brugt til at oprette det.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="6b7e6-115">Som en bedste fremgangsmåde kan du bruge et apple-id til administrationsopgaver og sørge for, at postkassen overvåges af mere end én person eller ved hjælp af en distributionsliste.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="6b7e6-116">Brug aldrig et personligt Apple-id.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="6b7e6-117">Brug det samme Apple-id til at forny Apple Push-certifikatet hver 12.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="6b7e6-118">Angiv det Apple-id, der bruges til at oprette dit Apple MDM-pushcertifikat.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="6b7e6-119">Registrer dette id som en påmindelse om, hvornår du skal forny certifikatet.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="6b7e6-120">Gå til certifikatfilen (.pem), vælg **Åbn**, og vælg derefter **Overfør**.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="6b7e6-121">Med push-certifikatet kan Intune tilmelde og administrere Apple-enheder.</span><span class="sxs-lookup"><span data-stu-id="6b7e6-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>