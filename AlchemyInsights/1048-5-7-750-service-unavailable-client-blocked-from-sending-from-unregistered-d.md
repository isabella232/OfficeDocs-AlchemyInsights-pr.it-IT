---
title: 1048 servizio 5.7.750 non disponibile. Client bloccato dall'invio di domini non registrati
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.openlocfilehash: 356bb008da3b08c320e6afde84c310629cc3be81
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/22/2019
ms.locfileid: "30208985"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="311c7-103">Client 5.7.750 bloccato dall'invio da un dominio non registrato</span><span class="sxs-lookup"><span data-stu-id="311c7-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="311c7-104">L'errore si verifica quando un volume elevato di messaggi viene inviato da domini che non sono provisioning in Office 365 (aggiunta come domini accettati e convalidati).</span><span class="sxs-lookup"><span data-stu-id="311c7-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="311c7-105">Per evitare questo errore, è possibile utilizzare un connettore del flusso di posta basato sui certificati in cui il dominio del certificato è un dominio di cui è stato effettuato il provisioning oppure eseguire il provisioning di tutti i domini di invio.</span><span class="sxs-lookup"><span data-stu-id="311c7-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

