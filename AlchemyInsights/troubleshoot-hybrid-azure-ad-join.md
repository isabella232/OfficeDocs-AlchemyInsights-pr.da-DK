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
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401901"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Fejlfinding af hybrid Azure AD-joinforbindelse

Anbefales kraftigt: Sørg for, at en enhed kan få adgang til enhedsregistreringsslutpunkter under systemkontoen ved hjælp af [scriptet Test enhedsregistreringsforbindelse.](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)

1. Hvis du konfigurerer enhedsregistrering for første gang, skal du sørge for at gennemgå I[ntro device management](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) i Azure Active Directory for at få mere at vide om, hvordan du får enheder under kontrol af Azure AD.
1. Hvis du registrerer enheder direkte i Azure AD og tilmelder dem i Intune, skal du først [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) sørge for, at du har konfigureret [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og licensering.
1. Sørg for, at du er autoriseret til at udføre handlinger i Azure AD og i det lokale AD. Kun en global administrator i Azure AD kan administrere indstillingerne for enhedsregistreringer. Hvis du konfigurerer automatiske registreringer i active directory i det lokale miljø, skal du desuden være administrator for Active Directory og AD FS (hvis det er relevant).

Hvis du vil have mere at vide om at løse potentielle problemer med hybrid joinforbindelse, skal du se Fejlfinding af [hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) joinforbindelse for at konfigurere hybrid Azure AD-enheder, der er forbundet og Administrer enheder ved hjælp af Azure Ad-portalen, under Konfigurer [hybride Azure AD-enheder (i](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) det lokale domæne) og Administrer enheder ved hjælp af [Azure-portalen.](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil løse almindelige problemer med hybrid Azure Active Directory-joinforbindelse (AD), skal du se [Ofte stillede spørgsmål om Hybrid Azure AD-joinforbindelse.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
