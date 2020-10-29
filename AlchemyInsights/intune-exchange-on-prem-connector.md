---
title: Connettore di Exchange locale di Intune
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
ms.contentlocale: it-IT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791523"
---
# <a name="intune-exchange-on-premise-connector"></a>Connettore di Exchange locale di Intune

Per informazioni dettagliate sulla configurazione del connettore tra Intune e Exchange ospitato in locale, vedere la documentazione seguente:

[Configurare il connettore di Exchange locale di Intune in Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Domande frequenti:**

D: viene visualizzato un errore, ad esempio "la versione del connettore di Exchange non è supportata" quando si tenta di configurare il connettore di Exchange. Quale potrebbe essere la causa?

A: l'account utilizzato viene concesso in licenza in modo appropriato-deve disporre di una licenza di Intune attiva

D: è possibile disporre di più connettori di Exchange?

A: è possibile configurare solo un connettore di Exchange per ogni tenant di Intune per ogni organizzazione di Exchange. Il connettore può essere installato solo in un server di un'organizzazione di Exchange con più server.

Inoltre, non è possibile disporre di connettori configurati sia per Exchange locale sia per Exchange Online configurati nello stesso tenant.

D: è possibile che il connettore utilizzi una matrice CAS come connessione a Exchange?

A: la specifica di una matrice CAS non è una configurazione supportata nell'installazione del connettore. È necessario specificare un solo server e deve essere hardcoded nel file di configurazione del connettore che può essere trovato in

Program Data\Microsoft\Microsoft Intune sul connettore di Exchange locale \ OnpremiseExchangeConnectorServiceConfiguration.xml

Individuare la voce seguente ```<ExchangeWebServiceURL />``` e sostituire l'URL con il server Exchange.

**Esempio**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Per ulteriori informazioni sulla risoluzione dei problemi, vedere la documentazione seguente: [risolvere i problemi del connettore di Exchange locale di Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Abilitazione della registrazione dettagliata per il connettore di Exchange**

1. Aprire il file di configurazione dell'analisi del connettore di Exchange per la modifica.  
Il file si trova in:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Esempio**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Individuare TraceSourceLine con la chiave seguente: OnPremisesExchangeConnectorService  
  
3. Modificare il valore del nodo SourceLevel da Information ActivityTracing (impostazione predefinita) a verbose ActivityTracing  

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
4. Riavviare il servizio Exchange di Microsoft Intune  
5. Sincronizzazione completa nel portale di Intune fino a quando non viene completata e quindi modificare nuovamente il codice XML in "Information ActivityTracing" e riavviare il servizio Exchange di Microsoft Intune.  
6. Il percorso dei registri è: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`