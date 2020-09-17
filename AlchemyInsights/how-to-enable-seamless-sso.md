---
title: Sådan aktiveres problemfrit SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780521"
---
# <a name="how-to-enable-seamless-sso"></a>Sådan aktiveres problemfrit SSO

Aktivér problemfrit SSO via [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Hvis du foretager en ny installation af Azure AD Connect, skal du vælge den [brugerdefinerede](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)installationssti. På logonsiden til **brugere** skal du vælge indstillingen **Aktivér enkeltlogon** .
  
Sådan kontrollerer du, at du har aktiveret problemfrit SSO korrekt:
  
1. Log på [Azure Active Directory administration](https://aad.portal.azure.com) som global administrator.

2. Vælg **Azure Active Directory** i venstre rude.

3. Kontrollér, at problemfrit enkeltlogon er **aktiveret**.

Hvis du vil have mere at vide, skal du se [Azure Active Directory problemfrit enkeltlogon: hurtig start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  