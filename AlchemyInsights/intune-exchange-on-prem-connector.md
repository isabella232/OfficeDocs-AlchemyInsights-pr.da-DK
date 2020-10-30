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
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-premise Connector

Hvis du vil have mere at vide om konfiguration af forbindelsen mellem Intune og Exchange, der er hosted lokalt, skal du se følgende dokumentation:

[Konfigurere den lokale Exchange Connector til Intune i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**OFTE**

Sp: Jeg får vist en fejl som "Exchange Connector-versionen understøttes ikke", når du forsøger at konfigurere Exchange Connector. Hvad kan være årsagen?

A: den konto, du bruger, er givet i licens til, den skal have en aktiv Intune-licens

Sp: er det muligt at have flere Exchange-forbindelser?

A: du kan kun konfigurere én Exchange-forbindelse pr. Intune-lejer pr. Exchange-organisation. Forbindelsen kan kun installeres på én server i en Exchange-organisation med flere servere.

Det er også muligt, at du ikke har konfigureret forbindelser for både Exchange on-premise og Exchange Online konfigureret i den samme lejer.

Sp: kan forbindelsen bruge en CAS-matrix som forbindelse til Exchange?

A: Hvis du angiver en CAS-matrix, er det ikke en understøttet konfiguration i forbindelses konfigurationen. Der skal kun angives en enkelt server, og det skal være hardcodede i forbindelses konfigurationsfilen, som kan findes i

program data\microsoft\microsoft Intune on premise Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Find den følgende post ```<ExchangeWebServiceURL />``` , og erstat URL-adressen med Exchange-serveren.

**:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Du kan finde flere oplysninger om fejlfinding i den følgende dokumentation: [fejlfinding af det lokale Exchange-forbindelsesprogram til Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivering af detaljeret logføring for Exchange Connector**

1. Åbn Exchange Connector Tracing-konfigurationsfilen til redigering.  
Filen er placeret på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Find TraceSourceLine med følgende nøgle: OnPremisesExchangeConnectorService  
  
3. Ændre SourceLevel-node værdien fra information ActivityTracing (standard) for at finde detaljerede ActivityTracing  

**:**
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
4. Genstart Microsoft Intune Exchange-tjenesten  
5. Fuld synkronisering i Intune-portalen, indtil den er fuldført, og ret derefter XML tilbage til "information ActivityTracing", og genstart Microsoft Intune-Exchange-tjenesten.  
6. Placeringen af logfilerne er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`