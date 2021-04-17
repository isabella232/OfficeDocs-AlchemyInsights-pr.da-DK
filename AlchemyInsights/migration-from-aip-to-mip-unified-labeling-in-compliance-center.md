---
title: Overførsel fra AIP til MIP/Unified Labeling i Overholdelsescenter
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825365"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Overførsel fra AIP til MIP/Unified Labeling i Overholdelsescenter

Hvis du vil overføre fra AIP-navne til samlet mærkning i Security and Compliance Center, skal du gøre følgende:

**Aktivér beskyttelse fra Azure-portalen**

1. Hvis du ikke allerede har gjort det, skal du åbne et nyt browservindue [og logge på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Gå til **Azure Information Protection-bladet.** Klik f.eks. på Alle tjenester i **hubmenuen,** og begynd at **skrive** Oplysninger i feltet Filter. Vælg **Azure Information Protection**. Hvis du ikke har åbnet Azure Information Protection-bladet [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) før, skal du se de ekstra engangstrin for at føje denne blade til portalen. Hvis du vil åbne Azure Information Protection-bladet, skal du enten have en [Azure Information Protection Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan, der omfatter Rights Management. Hvis du har et af disse abonnementer, men får vist en meddelelse om, at et gyldigt abonnement ikke kan findes, skal du kontakte [Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruge dine standard-supportkanaler.

2. Find **menuindstillingerne Administrer,** og vælg Beskyttelse **aktivering.** Klik **på Aktivér**, og bekræft derefter handlingen. Når aktiveringen er fuldført, vises Aktiveringen er **fuldført på informationslinjen.**

**Overfør Azure Information Protection-etiketter til Office 365 Security & Compliance Center**

1. Sørg for, at du er logget på som bruger med tilladelsen Global administrator.

2. Gå til **Azure Information Protection-bladet.**

3. Fra **menuindstillingen** Administrer skal du **vælge Samlet mærkat**.

4. På **Azure Information Protection – Samlet etiket blade skal du** klikke på **Aktivér og** følge onlinevejledningen.

**Bemærk!** Kontrollér, at du har de rette tilladelser, før du aktiverer sikkerheds- & Compliance Center-overførslen. Se disse artikler for at få flere oplysninger:

1. [Skal du være global administrator for at konfigurere Azure Information Protection, eller kan jeg uddelegere til andre administratorer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Vigtige oplysninger om administrative roller efter overførsel til Security & Compliance Center.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Du kan finde flere oplysninger om overførsel af AIP til Samlet mærkning til Security and Compliance Center under [Overfør navne](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
