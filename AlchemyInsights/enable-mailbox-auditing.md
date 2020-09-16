---
title: Aktivér overvågning af postkasse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806285"
---
# <a name="enable-mailbox-auditing"></a>Aktivér overvågning af postkasse

Hvis du vil aktivere postkasse overvågning for enten en enkelt bruger eller en hel organisation, skal følgende cmdletter køres fra Remote Power shell:
  
 **Enkelt bruger**
  
Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true
  
 **Markeds**
  
Get-postkassen-ResultSize ubegrænset-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true
  
[Lær mere](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

