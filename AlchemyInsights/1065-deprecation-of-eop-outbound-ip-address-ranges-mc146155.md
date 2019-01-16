---
title: 1065 negativi di EOP in uscita rangesMC146155 indirizzo IP
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296206"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="d1ee6-102">Rimozione di intervalli di indirizzi IP in uscita EOP</span><span class="sxs-lookup"><span data-stu-id="d1ee6-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="d1ee6-p101">È stato rilevato un problema potenziale con l'organizzazione che (se non è stata corretta per il 26 ottobre 2018) verificarsi problemi di flusso di posta al locale o destinazioni esterne. Come precedentemente comunicate per semplificare la gestione di intervallo di indirizzi IP, è stiamo consolidamento di intervalli di indirizzi IP di Exchange Online Protection (EOP) che vengono utilizzati per inviare e ricevere posta elettronica esterno a Office 365. Il nostro analisi indicano che una o più delle origini di posta elettronica esterno o delle destinazioni configurati nel connettori di flusso di posta elettronica non accettare connessioni dall'IP address intervalli illustrato [di seguito](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d1ee6-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="d1ee6-106">Agire prima del 26 ottobre per verificare che queste origini e destinazioni accetterà connessioni da e verso tutti [pubblicati gli indirizzi IP di EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d1ee6-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="d1ee6-107">Per ulteriori informazioni su questa modifica, vedere che Centro messaggi post [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="d1ee6-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="d1ee6-p102">**Nota**: se è stato utilizzato in precedenza IP o URL pubblicazione tramite HTML e XML RSS per gli aggiornamenti dell'endpoint, è inoltre necessario eseguire la migrazione ai nuovi servizi web per l'automazione di questi tipi di aggiornamenti. Per ulteriori informazioni, vedere [Office 365 endpoint categorie e indirizzo IP di Office 365 e il servizio web di URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="d1ee6-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

