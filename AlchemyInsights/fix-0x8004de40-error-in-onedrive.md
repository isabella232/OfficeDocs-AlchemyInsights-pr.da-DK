---
title: Ret 0x8004de40-fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745124"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Ret 0x8004de40-fejl i OneDrive

Hvis du modtager en 0x8004de40-fejl med OneDrive:

- Genstart den berørte computer, mens du har forbindelse til dit Acitve-katalog domæne.
- Hvis en genstart ikke løser problemet, kan du afbryde og genoprette forbindelsen til din enhed fra Azure AD. 

**Bemærk**: du skal være på dit virksomhedsnetværk, mens du udfører disse trin. Du skal ikke udføre disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f. eks. under rejser). 

- Åbn en kommandoprompt med administratorrettigheder. 
- Hvis du vil åbne en kommandoprompt med administratorrettigheder, skal du klikke på **Start**, højreklikke på **kommandoprompt**og derefter klikke på **Kør som administrator**.
- Skriv *dsregcmd/Leave* , og tryk på **Enter**.
- Når du er færdig, skal du skrive *dsregcmd/join* og trykke på **Enter**.
- Når du er færdig, skal du lukke kommandoprompten.
- Genstart computeren, og log på OneDrive.