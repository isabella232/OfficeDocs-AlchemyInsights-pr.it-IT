---
title: 1065 negativi di EOP in uscita rangesMC146155 indirizzo IP
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934888"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Rimozione di intervalli di indirizzi IP in uscita EOP

È stato rilevato un problema potenziale con l'organizzazione che (se non è stata corretta per il 26 ottobre 2018) verificarsi problemi di flusso di posta al locale o destinazioni esterne. Come precedentemente comunicate per semplificare la gestione di intervallo di indirizzi IP, è stiamo consolidamento di intervalli di indirizzi IP di Exchange Online Protection (EOP) che vengono utilizzati per inviare e ricevere posta elettronica esterno a Office 365. Il nostro analisi indicano che una o più delle origini di posta elettronica esterno o delle destinazioni configurati nel connettori di flusso di posta elettronica non accettare connessioni dall'IP address intervalli illustrato [di seguito](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Agire prima del 26 ottobre per verificare che queste origini e destinazioni accetterà connessioni da e verso tutti [pubblicati gli indirizzi IP di EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Per ulteriori informazioni su questa modifica, vedere che Centro messaggi post [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Nota**: se è stato utilizzato in precedenza IP o URL pubblicazione tramite HTML e XML RSS per gli aggiornamenti dell'endpoint, è inoltre necessario eseguire la migrazione ai nuovi servizi web per l'automazione di questi tipi di aggiornamenti. Per ulteriori informazioni, vedere [Office 365 endpoint categorie e indirizzo IP di Office 365 e il servizio web di URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

