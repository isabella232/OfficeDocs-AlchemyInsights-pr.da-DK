---
title: Fejlfinding af problemer med ejeren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900863"
---
# <a name="troubleshoot-owner-issues"></a>Fejlfinding af problemer med ejeren

Hvis du vil foretage fejlfinding af problemer med ejeren, skal du udføre følgende trin:

1. [Tilføje eller ændre Azure-abonnements administratorer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory-grupper (Azure ad)-grupper ejes og administreres af gruppe ejere. Gruppe ejere kan være brugere eller tjeneste principaler og kan administrere gruppen, herunder medlemskab. Kun eksisterende gruppe ejere eller gruppe-administrerende administratorer kan tildele gruppe ejere. Gruppe ejere behøver ikke at være medlem af gruppen.
2. [Tilføje eller ændre Azure-abonnements administratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): i denne artikel beskrives det, hvordan du kan tilføje eller ændre administratorrollen for en bruger ved hjælp af Azure RBAC på abonnements området.
3. Brug PowerShell til at tilføje en gruppeejer eller en program ejer.
