---
title: Fejlfinding af problemer med Azure AD-joinforbindelse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939913"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Fejlfinding af problemer med Azure AD-joinforbindelse

1. Hvis du konfigurerer enhedsregistrering for første gang, skal du kontrollere, at du har gennemgået Introduktion til enhedshåndtering i [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) der kan hjælpe dig med at få Enheder under kontrol til Azure AD. 
1. Hvis du registrerer enheder direkte i Azure AD og tilmelder dem i Intune, skal du sikre dig, at du har konfigureret [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) og har licensen på plads først. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)
1. Sørg for, at du er godkendt til at udføre handlinger i Azure AD. Kun en global administrator i Azure AD kan administrere indstillingerne for enhedsregistreringer.
1. Hvis du vil udføre implementering af Azure AD-joinforbindelse, skal [du se Planlæg Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Hvis du vil have mere at vide om at løse almindelige problemer med Azure AD-joinforbindelse, skal du se Ofte stillede spørgsmål om [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) Join og for Windows 10 Pro-enhed skal du se Kan ikke tilslutte Windows 10 Pro-maskine til Azure AD – du skal opgradere [til - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
