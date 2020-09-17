---
title: 1065 Deprecation de EOP l'indirizzo IP in uscita rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806799"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecazione degli intervalli di indirizzi IP in uscita di EOP

È stato rilevato un potenziale problema con l'organizzazione che (se non è stata corretta entro il 26 ottobre 2018) potrebbe interrompere il flusso di posta nelle destinazioni locali o esterne. Come precedentemente comunicato, per semplificare la gestione dell'intervallo di indirizzi IP, vengono consolidati gli intervalli di indirizzi IP di Exchange Online Protection (EOP) utilizzati per l'invio e la ricezione di messaggi di posta elettronica all'esterno di Microsoft 365. L'analisi indica che una o più origini di posta elettronica esterne o destinazioni configurate nei connettori del flusso di posta non accettano connessioni dagli intervalli di indirizzi IP riportati di [seguito](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act prima del 26 ottobre per garantire che queste origini e destinazioni accetteranno connessioni da e verso tutti [gli indirizzi IP di EOP pubblicati](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Per ulteriori informazioni su questa modifica, vedere Message Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Nota**: se in precedenza è stata utilizzata la pubblicazione IP o URL tramite HTML, XML e RSS per gli aggiornamenti degli endpoint, è inoltre necessario eseguire la migrazione ai nuovi servizi Web per automatizzare questi tipi di aggiornamenti. Per ulteriori informazioni, vedere [microsoft 365 endpoint Categories e microsoft 365 IP address and URL Web Service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
