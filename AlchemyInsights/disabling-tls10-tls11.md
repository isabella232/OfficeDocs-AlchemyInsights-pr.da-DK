---
title: Deaktivering af TLS1.0 og TLS 1.1 for SMTP AUTH-klientindsendelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/18/2021
ms.locfileid: "58454577"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Deaktivering af TLS1.0 og TLS 1.1 for SMTP AUTH-klientindsendelse

Vi er for nylig begyndt at deaktivere TLS1.0 og TLS 1.1 for SMTP AUTH-klientindsendelse. 

Hvis du har konfigureret en enhed, et program eller en server, der sender mails til Microsoft 365 ved hjælp af SMTP AUTH-klientafsendelsesmetoden, skal du kontrollere, at din enhed, dit program eller din server understøtter TLS 1.2 til SMTP. 