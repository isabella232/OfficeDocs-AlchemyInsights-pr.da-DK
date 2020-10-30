---
title: Intune Exchange on-premise Connector
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807400"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="6a49c-102">Intune Exchange on-premise Connector</span><span class="sxs-lookup"><span data-stu-id="6a49c-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="6a49c-103">Hvis du vil have mere at vide om konfiguration af forbindelsen mellem Intune og Exchange, der er hosted lokalt, skal du se følgende dokumentation:</span><span class="sxs-lookup"><span data-stu-id="6a49c-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="6a49c-104">Konfigurere den lokale Exchange Connector til Intune i Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="6a49c-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="6a49c-105">**OFTE**</span><span class="sxs-lookup"><span data-stu-id="6a49c-105">**FAQ:**</span></span>

<span data-ttu-id="6a49c-106">Sp: Jeg får vist en fejl som "Exchange Connector-versionen understøttes ikke", når du forsøger at konfigurere Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="6a49c-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="6a49c-107">Hvad kan være årsagen?</span><span class="sxs-lookup"><span data-stu-id="6a49c-107">What could be the cause?</span></span>

<span data-ttu-id="6a49c-108">A: den konto, du bruger, er givet i licens til, den skal have en aktiv Intune-licens</span><span class="sxs-lookup"><span data-stu-id="6a49c-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="6a49c-109">Sp: er det muligt at have flere Exchange-forbindelser?</span><span class="sxs-lookup"><span data-stu-id="6a49c-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="6a49c-110">A: du kan kun konfigurere én Exchange-forbindelse pr. Intune-lejer pr. Exchange-organisation.</span><span class="sxs-lookup"><span data-stu-id="6a49c-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="6a49c-111">Forbindelsen kan kun installeres på én server i en Exchange-organisation med flere servere.</span><span class="sxs-lookup"><span data-stu-id="6a49c-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="6a49c-112">Det er også muligt, at du ikke har konfigureret forbindelser for både Exchange on-premise og Exchange Online konfigureret i den samme lejer.</span><span class="sxs-lookup"><span data-stu-id="6a49c-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="6a49c-113">Sp: kan forbindelsen bruge en CAS-matrix som forbindelse til Exchange?</span><span class="sxs-lookup"><span data-stu-id="6a49c-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="6a49c-114">A: Hvis du angiver en CAS-matrix, er det ikke en understøttet konfiguration i forbindelses konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="6a49c-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="6a49c-115">Der skal kun angives en enkelt server, og det skal være hardcodede i forbindelses konfigurationsfilen, som kan findes i</span><span class="sxs-lookup"><span data-stu-id="6a49c-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="6a49c-116">program data\microsoft\microsoft Intune on premise Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="6a49c-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="6a49c-117">Find den følgende post ```<ExchangeWebServiceURL />``` , og erstat URL-adressen med Exchange-serveren.</span><span class="sxs-lookup"><span data-stu-id="6a49c-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="6a49c-118">**:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="6a49c-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="6a49c-119">Du kan finde flere oplysninger om fejlfinding i den følgende dokumentation: [fejlfinding af det lokale Exchange-forbindelsesprogram til Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="6a49c-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="6a49c-120">**Aktivering af detaljeret logføring for Exchange Connector**</span><span class="sxs-lookup"><span data-stu-id="6a49c-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="6a49c-121">Åbn Exchange Connector Tracing-konfigurationsfilen til redigering.</span><span class="sxs-lookup"><span data-stu-id="6a49c-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="6a49c-122">Filen er placeret på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="6a49c-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="6a49c-123">**:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="6a49c-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="6a49c-124">Find TraceSourceLine med følgende nøgle: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="6a49c-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="6a49c-125">Ændre SourceLevel-node værdien fra information ActivityTracing (standard) for at finde detaljerede ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="6a49c-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="6a49c-126">**:**</span><span class="sxs-lookup"><span data-stu-id="6a49c-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="6a49c-127">Genstart Microsoft Intune Exchange-tjenesten</span><span class="sxs-lookup"><span data-stu-id="6a49c-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="6a49c-128">Fuld synkronisering i Intune-portalen, indtil den er fuldført, og ret derefter XML tilbage til "information ActivityTracing", og genstart Microsoft Intune-Exchange-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="6a49c-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="6a49c-129">Placeringen af logfilerne er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="6a49c-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>