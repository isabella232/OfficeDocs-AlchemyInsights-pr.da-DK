---
title: Overførselstjenester – Flyt alle RDFE-tjenester til et andet abonnement
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940032"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Overførselstjenester – Flyt alle RDFE-tjenester til et andet abonnement

**Flyt ressourcer**

Azure-ressourcer kan flyttes til enten et andet Azure-abonnement eller en anden ressourcegruppe under det samme abonnement ved hjælp af Azure-portalen, Azure PowerShell, Azure CLI eller REST API for at flytte ressourcer.

Før du kan flytte ressourcer, skal du se:

- [Tjekliste før flytning af ressourcer](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjenester, der kan flyttes](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Sådan valideres flytningen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flyt vejledning til tjenester](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil flytte eksisterende ressourcer til en anden ressourcegruppe eller et andet abonnement, kan du bruge:

- [Azure-portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

[Selvstudium: Flytte Azure-ressourcer til en anden ressourcegruppe eller et andet abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Fejlfinding af fejl med Azure Resource Manager**

Se nedenstående artikler for at få mere at vide om nogle almindelige Azure-installationsfejl og modtage oplysninger om, hvordan du løser dem. Hvis du ikke kan finde fejlkoden for din installationsfejl, skal du se [Find fejlkode](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Fejlfinding af installationsfejl](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Fejlfinding i forbindelse med flytning af Azure-ressourcer til ny ressourcegruppe eller nyt abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Bemærk, at hvis du vil opgradere dit Azure-abonnement, f.eks. skifte fra gratis til pay-as-you-go, skal du konvertere dit abonnement.

- Hvis du vil opgradere en gratis prøveversion, skal du se Opgrader din [gratis prøveversion eller dit Microsoft Imagine Azure-abonnement til Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Hvis du vil ændre en pay-as-you-go-konto, skal du se Skift dit [Azure Pay-As-You-Go-abonnement til et andet tilbud.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Sådan tilføjer eller knytter du et Azure-abonnement til din Azure Active Directory lejer:**

1. Log på , og vælg det abonnement, du vil [bruge, på siden Abonnementer i Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Vælg **Skift mappe**.
3. Gennemse eventuelle advarsler, der vises, og vælg derefter **Rediger**.
4. Mappen ændres for abonnementet, og du får en vellykket meddelelse.
5. Brug *Mappeskifter* til at gå til din nye mappe. Det kan tage op til 10 minutter, før alt vises korrekt.

**Anbefalede dokumenter**

- [Overførsel af ejerskab af et Azure-abonnement](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flyt ressourcer til en ny ressourcegruppe eller et nyt abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Administrer ressourcer ved hjælp af Azure-portalen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
