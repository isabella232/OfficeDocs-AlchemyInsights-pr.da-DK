---
title: OneDrive logonfejl AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112906"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive logonfejl AADSTS50011

Hvis du får fejlmeddelelsen "AADSTS50011: Svarets URL-adresse, der er angivet i anmodningen, stemmer ikke overens med svaret", når du logger på OneDrive-appen, skal du kontrollere følgende:

Din OneDrive version skal være lig med eller større end version 20.052.XXXX.XXXX. Hvis du vil kontrollere din version, skal du klikke på det blå ikon OneDrive i meddelelsesområde vælge **Hjælp & Indstillinger > Indstillinger > Om**.

Dit netværk kan blokere for trafik **g.live.com** og **oneclient.sfx.ms**. Hvis denne trafik er blokeret, OneDrive ikke opdatere sig selv. Arbejd sammen med din netværksadministrator for at sikre, at du har adgang til disse URL-adresser. [Disse slutpunkter skal være](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) tilgængelige for kunder, der bruger Microsoft 365-planer.

Hvis du har brug for manuelt at få en aktuel version af OneDrive, skal du gå til [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
