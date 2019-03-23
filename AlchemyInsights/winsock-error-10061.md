---
title: 1554 Winsock-fejl 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772436"
---
# <a name="winsock-error-10061"></a>Winsock-fejl 10061

Denne fejlkode betyder, at Office 365 ikke kunne oprette en TCP socket (connection) med destinationsværten. Den mest sandsynlige årsag til denne fejl er et problem med firewallkonfigurationen af. Du kan løse problemet ved at kontrollere disse indstillinger:
  
- Kontrol firewall-konfiguration med oplysninger i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Hvis fejlen er bestemt til Exchange Online beskyttelse (EOP), skal du have tidligere meddelt en ændring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Kontroller, at din internetudbyder (ISP) ikke er blokerer for porten.
    
- Kontroller smart værten og målcomputerne serverindstillingerne i dine forbindelser.
    
Bemærk, at Office 365 ikke blokerer *indgående* forbindelser på denne måde. 
  

