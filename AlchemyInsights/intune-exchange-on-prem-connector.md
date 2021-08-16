---
title: Intune Exchange forbindelse i det lokale miljø
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013958"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange forbindelse i det lokale miljø

Du kan finde oplysninger om konfiguration af forbindelsen mellem Intune og Exchange, der hostes lokalt, i følgende dokumentation:

[Konfigurer Intune-forbindelsen i det lokale Exchange i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Ofte stillede spørgsmål:**

Sp: Jeg får vist en fejl, f.eks. "Versionen Exchange Forbindelse understøttes ikke", når jeg forsøger at konfigurere Exchange forbindelse. Hvad kan være årsagen?

A: Den konto, du bruger, har den korrekte licens – den skal have en aktiv Intune-licens

Sp: Er det muligt at have Exchange forbindelsesforbindelser?

A: Du kan kun konfigurere én Exchange forbindelse pr. Intune-lejer pr. Exchange organisation. Forbindelsen kan kun installeres på én server i en exchange-organisation med flere servere.

Du kan heller ikke have forbindelser konfigureret til Exchange lokale og lokale Exchange Online konfigureret i den samme lejer.

Sp: Kan forbindelsen bruge en CAS-matrix som forbindelse til Exchange?

A: Angivelse af en CAS-matrix understøttes ikke i konfigurationen af forbindelsen. Der skal kun angives en enkelt server, som skal være hardcoded i forbindelseskonfigurationsfilen, som kan findes i

programdata\microsoft\microsoft Intune i det lokale Exchange\ OnpremiseExchangeConnectorServiceConfiguration.xml

Find følgende post, ```<ExchangeWebServiceURL />``` og erstat URL-adressen med Exchange-serveren.

**Eksempel:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Se følgende dokumentation for yderligere fejlfinding: [Fejlfinding af intune i det lokale Exchange forbindelse](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivere detaljeret logføring for Exchange forbindelse**

1. Åbn konfigurationsfilen Exchange forbindelsessporing til redigering.  
Filen er placeret på: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Eksempel:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Find TraceSourceLine med følgende nøgle: OnPremisesExchangeConnectorService  
  
3. Skift nodeværdien SourceLevel fra Information ActivityTracing (standard) til Detaljeret aktivitet, der omfatter  

**Eksempel:**
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
4. Genstart Microsoft Intune Exchange tjeneste  
5. Fuld synkronisering i Intune Portal, indtil den er færdig, og skift derefter XML-koden tilbage til "Information ActivityTracing", og genstart Microsoft Intune Exchange Service.  
6. Placering af logfilerne er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`