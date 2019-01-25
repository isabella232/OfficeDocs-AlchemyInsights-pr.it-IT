---
title: Accesso negato durante la visualizzazione di un flusso di lavoro
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475860"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accesso negato durante la visualizzazione di un flusso di lavoro

SharePoint 2013 i flussi di lavoro tenta di inviare un messaggio di posta elettronica a un gruppo di SharePoint può non riuscire con un messaggio di errore "Accesso negato" se l'appartenenza del gruppo di SharePoint non è impostata su tutti gli utenti.
  
 **Per risolvere questo problema, eseguire la procedura seguente:**
  
 1. Consentire a tutti i partecipanti di visualizzare i membri del gruppo di SharePoint. 
  
 2. Rimuovere il gruppo di SharePoint da a o CC riga del messaggio di posta elettronica. 
  
 3. Aggiungere esplicitamente gli utenti a o CC linea se non può essere modificata la visibilità l'appartenenza al gruppo di SharePoint. 
  
Per visualizzare ulteriori informazioni, consultare [HTTP non autorizzato a /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

