---
title: Monitoraggio dell'accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418473"
---
# <a name="monitoring-conditional-access"></a>Monitoraggio dell'accesso condizionale

Gli utenti a cui viene assegnato l'accesso condizionale ricevono un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il testo, è consigliabile eseguire una o più delle soluzioni seguenti:
  
- Se si presume che il dispositivo venga registrato, avvisare l'utente di accedere all'app portale aziendale e verificare che venga visualizzato nel portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
    
- Nel portale di Azure passare a **Intune \> Device Compliance**. In **Monitor** fare clic su **conformità dispositivo**. Visualizzare il rapporto di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme. 
    
- Nel portale di Azure passare a **Intune \> Device Compliance**. In **Gestisci**fare clic su **criteri**. Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente. Se non è stato assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo. 
    
- Modificare l'assegnazione di accesso condizionale dell'utente.
    
1. Nel portale di Azure passare ai **criteri \> di accesso \> condizionale di Intune**
    
2. Selezionare un criterio dall'elenco
    
3. Fare clic su **utenti e gruppi**
    
4. Per assegnare un determinato criterio a un utente, aggiungerli all' **** elenco Includi. Per assicurarsi che una persona venga omessa dal criterio, aggiungerla all'elenco **Escludi** . 
    
Per ulteriori informazioni [, vedere: come monitorare i dispositivi di accesso condizionale](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

