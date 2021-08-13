---
title: Fejlfinding af hybrid Azure AD-joinforbindelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939265"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Fejlfinding af hybrid Azure AD-joinforbindelse

Meget anbefalet Sørg for, at en enhed kan få adgang til enhedsregistreringsslutpunkter under systemkontoen ved hjælp af [scriptet Test enhedsregistreringsforbindelse](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Hvis du konfigurerer enhedsregistreringer for første gang, skal du sørge for at gennemgå Jeg[er ikke-introduktion](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) til enhedshåndtering i Azure Active Directory for at få mere at vide om, hvordan du får enheder under kontrol i Azure AD.
1. Hvis du registrerer enheder direkte i Azure AD og tilmelder dem i Intune, skal du sørge [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) for, at du har [konfigureret Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og har licensen på plads først.
1. Sørg for, at du er autoriseret til at udføre handlinger i Azure AD og i det lokale AD. Kun en global administrator i Azure AD kan administrere indstillingerne for enhedsregistreringer. Hvis du konfigurerer automatiske registreringer i dit lokale Active Directory, skal du desuden være administrator for Active Directory og AD FS (hvis det er relevant).

Hvis du vil have mere at vide om at løse potentielle problemer med hybrid joinforbindelse, skal du se Fejlfinding af [hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) joinforbindelse for at konfigurere hybrid Azure AD-enheder, der er forbundet og Administrere enheder ved hjælp af Azure Ad-portalen, se Konfigurer [hybride Azure AD-enheder (på](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) stedet for domæne sammenføjede) enheder og Administrer enheder ved hjælp af [Azure-portalen.](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil løse almindelige problemer med hybrid Azure Active Directory (AD)-joinforbindelse, skal du se Ofte [stillede spørgsmål om Azure AD-hybridforbindelse.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
