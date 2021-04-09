---
title: Ret 0x8004de40 fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649742"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Ret 0x8004de40 fejl i OneDrive

Hvis du kører Windows 7 og modtager denne fejl, skal du opdatere for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows.

Hvis du kører Windows 10, og du modtager en fejlmeddelelse 0x8004de40 med OneDrive:

- Genstart den påvirkede computer, mens du har forbindelse til dit Acitve-mappedomæne.
- Hvis en genstart ikke løser problemet, skal du fjerne forbindelse til og slutte enheden til din enhed igen fra Azure AD. 

**Bemærk!** Du bør være på virksomhedens netværk, mens du udfører disse trin. Udfør ikke disse trin, når du ikke har forbindelse til virksomhedens infrastruktur (f.eks. mens du rejser). 

1. Åbn en kommandoprompt med administratorrettigheder ved at vælge **Start**, højreklik **på Kommandoprompt**, og vælg **derefter Kør som administrator**.

1. Skriv *dsregcmd /leave, og* tryk på **Enter.**

1. Når du er færdig, skal *du skrive dsregcmd /join* og trykke på **Enter.**

1. Luk kommandoprompten, når du er færdig.

1. Genstart computeren, og log på OneDrive.