---
title: Afhjælp fejlen Programmet blev ikke fundet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810478"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="1c170-102">Afhjælp fejlen "Programmet blev ikke fundet"</span><span class="sxs-lookup"><span data-stu-id="1c170-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="1c170-103">Appinstallationsfejlen "Programmet blev ikke registreret efter vellykket installation", som blev blevet rapporteret af Intune, kan forekomme på alle overordnede OS-platforme (Windows, iOS og Android).</span><span class="sxs-lookup"><span data-stu-id="1c170-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="1c170-104">De mest almindelige scenarier, der genererer denne fejl, omfatter:</span><span class="sxs-lookup"><span data-stu-id="1c170-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="1c170-105">Appen er blevet opdateret uden for Intune (fra en appstore fra tredjepart) efter den indledende installation.</span><span class="sxs-lookup"><span data-stu-id="1c170-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="1c170-106">For eksempel kan nogle programmer som f.eks. Google Chrome udføre automatiske opdateringer.</span><span class="sxs-lookup"><span data-stu-id="1c170-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="1c170-107">En bruger har fjernet appen efter den indledende installation.</span><span class="sxs-lookup"><span data-stu-id="1c170-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="1c170-108">Hvis du vil løse dette problem, skal du først foretage en gennemgang af de berørte enheder for at fastslå det scenarie, hvor fejlen opstår.</span><span class="sxs-lookup"><span data-stu-id="1c170-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="1c170-109">Hvis appen er blevet opdateret uden for Intune, kan app-installationen indstilles til at ignorere programversionen.</span><span class="sxs-lookup"><span data-stu-id="1c170-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="1c170-110">Hvis du vil gøre dette, skal du under **Konfiguration af apps > App-oplysninger** indstille **Ignorer app-** version til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="1c170-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="1c170-111">Når du målretter klienten, kan det være relevant at installere programmet som "obligatorisk", og sikre, at den nyeste version installeres.</span><span class="sxs-lookup"><span data-stu-id="1c170-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="1c170-112">Alternativt kan man på iOS-platformen bruge funktionen **Automatiske opdateringer**, der er knyttet til Apple Volume Purchase-programmet, som kan konfigureres til automatisk at opdatere til nye programversioner, når de bliver tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="1c170-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="1c170-113">Hvis du vil have mere at vide om fejlfinding af problemer med app-installation, skal du se [Fejlfinding af problemer med app-installation](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="1c170-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
