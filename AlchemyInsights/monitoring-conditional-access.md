---
title: Monitoraggio accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656571"
---
# <a name="monitoring-conditional-access"></a>Monitoraggio accesso condizionale

Se non soddisfano i requisiti dell'organizzazione access, gli utenti assegnati con accesso condizionale riceveranno un messaggio di posta elettronica di notifica. Per risolvere, è consigliabile una o più delle soluzioni seguenti:
  
- Se il dispositivo presumendo che iscritto, consigliare all'utente di accedere all'applicazione portale della società e verificare che venga visualizzato nel portale della società. In caso contrario, l'utente deve registrare il dispositivo.
    
- Nel portale di Azure passare a **Intune \> conformità dispositivo**. In **Monitor** fare clic su **dispositivo conformità**. Visualizzare il report di conformità di dispositivo per verificare che il dispositivo dell'utente è contrassegnato come compatibile. 
    
- Nel portale di Azure passare a **Intune \> conformità dispositivo**. In **Gestione**fare clic su **criteri**. Nell'elenco dei criteri di conformità, verificare che un profilo viene assegnato al dispositivo dell'utente. Se non viene assegnato alcun profilo, Intune non sarà in grado di verificare lo stato della conformità del dispositivo. 
    
- Modificare l'assegnazione di accesso condizionato dell'utente.
    
1. Nel portale di Azure passare a **Intune \> accesso condizionato \> criteri**
    
2. Selezionare un criterio nell'elenco
    
3. Fare clic su **utenti e gruppi**
    
4. Per un determinato criterio a un utente di destinazione, aggiungerli all'elenco di **inclusione** . Per garantire che un utente viene omesso il parametro dal criterio, aggiungerli all'elenco di **esclusione** . 
    
Ulteriori: [come monitorare gli accessi condizionale dispositivi](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

