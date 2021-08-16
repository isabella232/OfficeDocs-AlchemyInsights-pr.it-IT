---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031266"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecazione degli intervalli di indirizzi IP in uscita di EOP

È stato rilevato un potenziale problema con l'organizzazione che , se non è stato corretto entro il 26 ottobre 2018, potrebbe interrompere il flusso di posta verso le destinazioni locali o esterne. Come comunicato in precedenza, per semplificare la gestione degli intervalli di indirizzi IP, stiamo consolidando gli intervalli di indirizzi IP di Exchange Online Protection (EOP) utilizzati per inviare e ricevere posta elettronica all'esterno di Microsoft 365. L'analisi indica che una o più origini o destinazioni di posta elettronica esterne configurate nei connettori del flusso di posta non accettano connessioni dagli intervalli di indirizzi IP [mostrati qui.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Agire prima del 26 ottobre per garantire che queste origini e destinazioni accettino connessioni da e verso tutti gli indirizzi [IP EOP pubblicati.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Per ulteriori informazioni su questa modifica, vedere Post del Centro messaggi [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Nota:** se in precedenza è stata utilizzata la pubblicazione di IP o URL tramite HTML, XML e RSS per gli aggiornamenti degli endpoint, è consigliabile eseguire anche la migrazione ai nuovi servizi Web per automatizzare questi tipi di aggiornamenti. Per ulteriori informazioni, vedere Microsoft 365 di endpoint e [Microsoft 365 servizio Web INDIRIZZO IP e URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
