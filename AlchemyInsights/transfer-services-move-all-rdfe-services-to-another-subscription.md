---
title: Overføre tjenester-flytte alle RDFE-tjenester til et andet abonnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691978"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Overføre tjenester-flytte alle RDFE-tjenester til et andet abonnement

**Flytte ressourcer**

Azure-ressourcer kan flyttes til enten et andet Azure-abonnement eller en ressourcegruppe under det samme abonnement ved hjælp af Azure-portalen, Azure PowerShell, Azure CLI eller The REST API til at flytte ressourcer.

Før du kan flytte ressourcer, skal du se:

- [Tjekliste før flytning af ressourcer](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjenester, der kan flyttes](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Sådan valideres flytningen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flyt vejledning til tjenester](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil flytte eksisterende ressourcer til en anden ressourcegruppe eller et abonnement, kan du bruge:

- [Azure-Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Selvstudium: [flytte Azure-ressourcer til en anden ressourcegruppe eller et andet abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Fejlfinding af fejl med Azure Resource Manager**

Se artiklerne nedenfor for at få mere at vide om nogle almindelige Azure-installationsfejl og modtag oplysninger for at løse dem. Hvis du ikke kan finde fejlkoden for installations fejlen, skal du se [finde fejlkode](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Fejlfinding af installationsfejl](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Fejlfinding ved flytning af Azure-ressourcer til en ny ressourcegruppe eller et abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Bemærk, at hvis du vil opgradere dit Azure-abonnement, f. eks Skift fra at betale til at blive, skal du konvertere dit abonnement.

- Hvis du vil opgradere en gratis prøveversion, skal du se [opgradere din gratis prøveversion eller Microsoft Forestil dig Azure-abonnement for at betale som dig](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Hvis du vil ændre en løn som din Go-konto, skal du se [ændre dit abonnement på Azure-pay-Go-Go til et andet bud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Sådan tilføjer eller knytter du et Azure-abonnement til din Azure Active Directory-lejer:**

1. Log på, og vælg det abonnement, du vil bruge, på [siden abonnementer i Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Vælg **Skift mappe**.
3. Gennemse eventuelle advarsler, der vises, og vælg derefter **Rediger**.
4. Mappen er ændret for abonnementet, og du får en meddelelse om succes.
5. Brug *mappen* skifteren til at gå til den nye mappe. Det kan tage op til 10 minutter, før alt vises korrekt.

**Anbefalede dokumenter**

- [Overføre ejerskabet af et Azure-abonnement](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flytte ressourcer til en ny ressourcegruppe eller et abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Administrere ressourcer ved hjælp af Azure-portalen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
