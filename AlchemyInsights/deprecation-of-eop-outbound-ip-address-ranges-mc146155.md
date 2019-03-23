---
title: 1065 Deprecation de EOP l'indirizzo IP in uscita rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777276"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="e37b1-102">Deprecazione degli intervalli di indirizzi IP in uscita di EOP</span><span class="sxs-lookup"><span data-stu-id="e37b1-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="e37b1-103">È stato rilevato un potenziale problema con l'organizzazione che (se non è stata corretta entro il 26 ottobre 2018) potrebbe interrompere il flusso di posta nelle destinazioni locali o esterne.</span><span class="sxs-lookup"><span data-stu-id="e37b1-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="e37b1-104">Come precedentemente comunicato, per semplificare la gestione degli intervalli di indirizzi IP, è possibile consolidare gli intervalli di indirizzi IP di Exchange Online Protection (EOP) utilizzati per inviare e ricevere messaggi di posta elettronica all'esterno di Office 365.</span><span class="sxs-lookup"><span data-stu-id="e37b1-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="e37b1-105">L'analisi indica che una o più origini di posta elettronica esterne o destinazioni configurate nei connettori del flusso di posta non accettano connessioni dagli intervalli di indirizzi IP riportati di [seguito](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="e37b1-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="e37b1-106">Act prima del 26 ottobre per garantire che queste origini e destinazioni accetteranno connessioni da e verso tutti [gli indirizzi IP di EOP pubblicati](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="e37b1-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="e37b1-107">Per ulteriori informazioni su questa modifica, vedere Message Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="e37b1-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="e37b1-108">**Nota**: se in precedenza è stata utilizzata la pubblicazione IP o URL tramite HTML, XML e RSS per gli aggiornamenti degli endpoint, è inoltre necessario eseguire la migrazione ai nuovi servizi Web per automatizzare questi tipi di aggiornamenti.</span><span class="sxs-lookup"><span data-stu-id="e37b1-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="e37b1-109">Per ulteriori informazioni, vedere [office 365 categorie endpoint e office 365 IP address and URL Web Service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="e37b1-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

