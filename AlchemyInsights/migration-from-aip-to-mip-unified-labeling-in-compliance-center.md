---
title: Overførsel fra AIP til MIP/samlet mærkning i overholdelses Center
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674320"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Overførsel fra AIP til MIP/samlet mærkning i overholdelses Center

Hvis du vil overføre fra AIP-navne til samlet Etiketing i sikkerheds-og Overholdelsescenter, skal du gøre følgende:

**Aktivere beskyttelse fra Azure-portalen**

1. Hvis du ikke allerede har gjort det, skal du åbne et nyt browservindue og [logge på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Gå til bladet **Azure information Protection** . I menuen hub skal du for eksempel klikke på **alle tjenester** og begynde at skrive **oplysninger** i feltet Filter. Vælg **Azure information Protection**. Hvis du ikke har åbnet bladet til Azure-informations beskyttelse før, skal du se de [trin](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , der er en gang til at føje denne kørsel til portalen. Hvis du vil åbne bladet til Azure-beskyttelse af oplysninger, skal du enten have en [Azure-informations beskyttelses-Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan, der omfatter rettighedsstyring. Hvis du har et af disse abonnementer, men se en meddelelse om, at et gyldigt abonnement ikke kan findes, skal du [kontakte Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruge standard support kanalerne.

2. Find indstillinger for menuen **Administrer** , og vælg **beskyttelse af aktiver**. Klik på **Aktivér**, og bekræft derefter din handling. Når aktiveringen er fuldført, viser informationslinjen **aktiveringen fuldført**.

**Overføre Azure information Protection-etiketter til Office 365 Security & Compliance Center**

1. Kontrollér, at du er logget på som bruger med Global administrator tilladelse.

2. Gå til bladet **Azure information Protection** .

3. I menuen **Administrer** skal du vælge **samlet etiketing**.

4. På bladet **Azure information Protection-samlet etikette** ring skal du klikke på **Aktivér** og følge instruktionerne online.

**Bemærk**! Kontrollér, at du har de rette tilladelser, før du aktiverer overflytning af sikkerheds & Compliance Center. Du kan finde flere oplysninger i disse artikler:

1. [Skal du være global administrator for at konfigurere Azure information Protection eller kan jeg uddelegere til andre administratorer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Vigtige oplysninger om administrative roller, når du har overført til sikkerheds & overholdelses Center.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Hvis du vil have mere at vide om AIP til at give samlet etikettering til sikkerheds-og overholdelses Center, skal du se [overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
