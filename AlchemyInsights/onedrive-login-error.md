---
title: Fejl AADSTS50011 for OneDrive-logon
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982446"
---
# <a name="onedrive-login-error-aadsts50011"></a>Fejl AADSTS50011 for OneDrive-logon

Hvis du modtager en fejl "AADSTS50011: svar-URL-adressen, der er angivet i anmodningen, ikke stemmer overens med svaret" ved signering i OneDrive-appen, skal du kontrollere følgende:

Din version af OneDrive skal være lig med eller større end version 20.052. XXXX. XX. Hvis du vil kontrollere din version, skal du klikke på det blå OneDrive-ikon i meddelelsesområdet, vælge **hjælp & indstillinger > indstillinger > om**.

Dit netværk kan blokere for trafik til **g.live.com** -og **oneclient.SFX.MS**. Hvis den pågældende trafik blokeres, kan OneDrive ikke opdatere sig selv. Samarbejd med din netværksadministrator for at sikre, at du har adgang til disse URL-adresser. [Disse slutpunkter](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) skal være tilgængelige for kunder, der bruger Microsoft 365-planer.

Hvis du har brug for at hente en aktuel version af OneDrive manuelt, skal du gå til [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
