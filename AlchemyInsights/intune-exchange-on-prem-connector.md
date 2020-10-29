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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="c5858-102">Connettore di Exchange locale di Intune</span><span class="sxs-lookup"><span data-stu-id="c5858-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="c5858-103">Per informazioni dettagliate sulla configurazione del connettore tra Intune e Exchange ospitato in locale, vedere la documentazione seguente:</span><span class="sxs-lookup"><span data-stu-id="c5858-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="c5858-104">Configurare il connettore di Exchange locale di Intune in Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="c5858-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="c5858-105">**Domande frequenti:**</span><span class="sxs-lookup"><span data-stu-id="c5858-105">**FAQ:**</span></span>

<span data-ttu-id="c5858-106">D: viene visualizzato un errore, ad esempio "la versione del connettore di Exchange non è supportata" quando si tenta di configurare il connettore di Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5858-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="c5858-107">Quale potrebbe essere la causa?</span><span class="sxs-lookup"><span data-stu-id="c5858-107">What could be the cause?</span></span>

<span data-ttu-id="c5858-108">A: l'account utilizzato viene concesso in licenza in modo appropriato-deve disporre di una licenza di Intune attiva</span><span class="sxs-lookup"><span data-stu-id="c5858-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="c5858-109">D: è possibile disporre di più connettori di Exchange?</span><span class="sxs-lookup"><span data-stu-id="c5858-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="c5858-110">A: è possibile configurare solo un connettore di Exchange per ogni tenant di Intune per ogni organizzazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5858-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="c5858-111">Il connettore può essere installato solo in un server di un'organizzazione di Exchange con più server.</span><span class="sxs-lookup"><span data-stu-id="c5858-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="c5858-112">Inoltre, non è possibile disporre di connettori configurati sia per Exchange locale sia per Exchange Online configurati nello stesso tenant.</span><span class="sxs-lookup"><span data-stu-id="c5858-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="c5858-113">D: è possibile che il connettore utilizzi una matrice CAS come connessione a Exchange?</span><span class="sxs-lookup"><span data-stu-id="c5858-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="c5858-114">A: la specifica di una matrice CAS non è una configurazione supportata nell'installazione del connettore.</span><span class="sxs-lookup"><span data-stu-id="c5858-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="c5858-115">È necessario specificare un solo server e deve essere hardcoded nel file di configurazione del connettore che può essere trovato in</span><span class="sxs-lookup"><span data-stu-id="c5858-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="c5858-116">Program Data\Microsoft\Microsoft Intune sul connettore di Exchange locale \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c5858-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="c5858-117">Individuare la voce seguente ```<ExchangeWebServiceURL />``` e sostituire l'URL con il server Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5858-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="c5858-118">**Esempio**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="c5858-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="c5858-119">Per ulteriori informazioni sulla risoluzione dei problemi, vedere la documentazione seguente: [risolvere i problemi del connettore di Exchange locale di Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="c5858-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="c5858-120">**Abilitazione della registrazione dettagliata per il connettore di Exchange**</span><span class="sxs-lookup"><span data-stu-id="c5858-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="c5858-121">Aprire il file di configurazione dell'analisi del connettore di Exchange per la modifica.</span><span class="sxs-lookup"><span data-stu-id="c5858-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="c5858-122">Il file si trova in:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c5858-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="c5858-123">**Esempio**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="c5858-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="c5858-124">Individuare TraceSourceLine con la chiave seguente: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="c5858-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="c5858-125">Modificare il valore del nodo SourceLevel da Information ActivityTracing (impostazione predefinita) a verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="c5858-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="c5858-126">**Esempio:**</span><span class="sxs-lookup"><span data-stu-id="c5858-126">**Example:**</span></span>
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
4. <span data-ttu-id="c5858-127">Riavviare il servizio Exchange di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c5858-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="c5858-128">Sincronizzazione completa nel portale di Intune fino a quando non viene completata e quindi modificare nuovamente il codice XML in "Information ActivityTracing" e riavviare il servizio Exchange di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c5858-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="c5858-129">Il percorso dei registri è: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="c5858-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>