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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="49eb1-102">Fejlfinding af AADSTS-fejlkoder (Azure AD Authentication and Authorization)</span><span class="sxs-lookup"><span data-stu-id="49eb1-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="49eb1-103">Udfør følgende anbefalede trin for at løse AAD-godkendelses- og godkendelsesfejlkoder (AADSTS):</span><span class="sxs-lookup"><span data-stu-id="49eb1-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="49eb1-104">**Håndtering af fejlkoder i dit program**</span><span class="sxs-lookup"><span data-stu-id="49eb1-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="49eb1-105">**OAuth2.0-specifikationerne**, giver vejledning til, hvordan du håndterer fejl under godkendelse ved hjælp af https://tools.ietf.org/html/rfc6749#section-5.2 fejldelen af fejlsvaret.</span><span class="sxs-lookup"><span data-stu-id="49eb1-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="49eb1-106">**fejl:** En fejlkodestreng, der kan bruges til at klassificere typer af fejl, der opstår, og som skal bruges til at reagere på fejl.</span><span class="sxs-lookup"><span data-stu-id="49eb1-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="49eb1-107">**Fejlfeltet** har flere mulige værdier – gennemse linkene til protokoldokumentationen og OAuth 2.0-specifikationerne for at få flere oplysninger om bestemte fejl, og hvordan du kan reagere på dem.</span><span class="sxs-lookup"><span data-stu-id="49eb1-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="49eb1-108">Her er et eksempel på et fejlsvar:</span><span class="sxs-lookup"><span data-stu-id="49eb1-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="49eb1-109">**Oplysninger om den aktuelle opslagsfejlkode**</span><span class="sxs-lookup"><span data-stu-id="49eb1-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="49eb1-110">Fejlkoder og meddelelser kan blive ændret.</span><span class="sxs-lookup"><span data-stu-id="49eb1-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="49eb1-111">Du kan finde de seneste oplysninger på siden for at finde https://login.microsoftonline.com/error AADSTS-fejlbeskrivelser, løsninger og nogle foreslåede løsninger.</span><span class="sxs-lookup"><span data-stu-id="49eb1-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="49eb1-112">Du kan også søge efter og foretage fejlfinding af [AADSTS-fejlkoder,](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) der er angivet i artiklen [Azure AD-godkendelses- og godkendelsesfejlkoder.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="49eb1-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="49eb1-113">**Få hjælp**</span><span class="sxs-lookup"><span data-stu-id="49eb1-113">**Get Help**</span></span>

- <span data-ttu-id="49eb1-114">[Support- og hjælpemuligheder for](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) udviklere – Hvis du har brug for et svar på et spørgsmål eller hjælp til at løse et problem, der ikke er dækket af vores dokumentation, kan det være tid til at kontakte eksperter for at få hjælp.</span><span class="sxs-lookup"><span data-stu-id="49eb1-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="49eb1-115">Denne artikel indeholder flere forslag til at få svar på dine spørgsmål, når du udvikler apps, der integreres med Microsoft-identitetsplatformen.</span><span class="sxs-lookup"><span data-stu-id="49eb1-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








