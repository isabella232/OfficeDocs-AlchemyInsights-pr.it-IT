---
title: Accesso negato durante la visualizzazione di un flusso di lavoro
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687334"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accesso negato durante la visualizzazione di un flusso di lavoro

I flussi di lavoro di SharePoint 2013 che tentano di inviare un messaggio di posta elettronica a un gruppo di SharePoint non possono avere esito positivo se l'appartenenza al gruppo di SharePoint non è impostata su tutti.
  
 **Per risolvere il problema, eseguire la procedura seguente:**
  
 1. Consentire a tutti di visualizzare i membri del gruppo di SharePoint.
  
 2. Rimuovere il gruppo di SharePoint dalla riga a o CC del messaggio di posta elettronica.
  
 3. Aggiungere in modo esplicito gli utenti alla riga a o CC se la visibilità di appartenenza non può essere modificata per il gruppo di SharePoint.
  
Per visualizzare ulteriori dettagli, fare riferimento a [http non autorizzato a/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  