---
title: Fejlfinding af AADSTS-fejlkoder (Azure AD Authentication and Authorization)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035635"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Fejlfinding af AADSTS-fejlkoder (Azure AD Authentication and Authorization)

Udfør følgende anbefalede trin for at løse AAD-godkendelses- og godkendelsesfejlkoder (AADSTS):

1. **Håndtering af fejlkoder i dit program**

- **OAuth2.0-specifikationerne**, giver vejledning til, hvordan du håndterer fejl under godkendelse ved hjælp af https://tools.ietf.org/html/rfc6749#section-5.2 fejldelen af fejlsvaret.

    - **fejl:** En fejlkodestreng, der kan bruges til at klassificere typer af fejl, der opstår, og som skal bruges til at reagere på fejl.
    - **Fejlfeltet** har flere mulige værdier – gennemse linkene til protokoldokumentationen og OAuth 2.0-specifikationerne for at få flere oplysninger om bestemte fejl, og hvordan du kan reagere på dem.

- Her er et eksempel på et fejlsvar:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Oplysninger om den aktuelle opslagsfejlkode**

- Fejlkoder og meddelelser kan blive ændret. Du kan finde de seneste oplysninger på siden for at finde https://login.microsoftonline.com/error AADSTS-fejlbeskrivelser, løsninger og nogle foreslåede løsninger.
- Du kan også søge efter og foretage fejlfinding af [AADSTS-fejlkoder,](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) der er angivet i artiklen [Azure AD-godkendelses- og godkendelsesfejlkoder.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Få hjælp**

- [Support- og hjælpemuligheder for](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) udviklere – Hvis du har brug for et svar på et spørgsmål eller hjælp til at løse et problem, der ikke er dækket af vores dokumentation, kan det være tid til at kontakte eksperter for at få hjælp. Denne artikel indeholder flere forslag til at få svar på dine spørgsmål, når du udvikler apps, der integreres med Microsoft-identitetsplatformen.








