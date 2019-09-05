---
title: Aktivér overvågning af postkasse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736247"
---
# <a name="enable-mailbox-auditing"></a>Aktivér overvågning af postkasse

Hvis du vil aktivere postkasseovervågning for enten en enkelt bruger eller en hel organisation, skal følgende cmdletter køres fra Remote Power shell:
  
 **Enkelt bruger**
  
Set-postkasse-identitet "Jane Dow"-AuditEnabled $true
  
 **Organisation**
  
Hent-postkasse-ResultSize ubegrænset-filter {RecipientTypeDetails-EQ "User Mailbox"} | Set-Mailbox-AuditEnabled $true
  
[Lær mere](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

