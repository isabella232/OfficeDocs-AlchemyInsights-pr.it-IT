---
title: Intune Exchange connettore locale
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
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013968"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange connettore locale

Per informazioni dettagliate sulla configurazione del connettore tra Intune e Exchange ospitata in locale, vedere la documentazione seguente:

[Configurare il connettore di Exchange intune locale in Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Domande frequenti:**

D: Viene visualizzato un errore come "La versione del connettore di Exchange non è supportata" quando si tenta di configurare il Exchange connettore. Quale potrebbe essere la causa?

A: L'account in uso è concesso in licenza in modo appropriato- deve disporre di una licenza di Intune attiva

D: È possibile avere più Exchange connettori?

A: È possibile configurare un solo connettore Exchange per ogni tenant di Intune per Exchange organizzazione. Il connettore può essere installato solo in un server in un'organizzazione di exchange con più server.

Inoltre, non è possibile configurare connettori per Exchange locale e Exchange Online nello stesso tenant.

D: Il connettore può utilizzare una matrice CAS come connessione a Exchange?

A: La specifica di una matrice CAS non è una configurazione supportata nella configurazione del connettore. Deve essere specificato un solo server e deve essere hardcoded nel file di configurazione del connettore disponibile in

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Individuare la voce seguente ```<ExchangeWebServiceURL />``` e sostituire l'URL con il server Exchange.

**Esempio:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Per ulteriori informazioni sulla risoluzione dei problemi, vedere la documentazione seguente: Risolvere i problemi del connettore di Exchange [Intune locale](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Abilitazione della registrazione dettagliata per il Exchange connettore**

1. Aprire il file di Exchange di traccia del connettore per la modifica.  
Il file si trova in : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Esempio:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Individuare TraceSourceLine con la chiave seguente: OnPremisesExchangeConnectorService  
  
3. Modificare il valore del nodo SourceLevel da Information ActivityTracing (impostazione predefinita) a Verbose ActivityTracing  

**Esempio:**
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
4. Riavviare il Microsoft Intune Exchange servizio  
5. Sincronizzazione completa nel portale di Intune fino al termine e quindi modificare il codice XML in "Information ActivityTracing" e riavviare il Microsoft Intune Exchange Service.  
6. Il percorso dei registri è: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`