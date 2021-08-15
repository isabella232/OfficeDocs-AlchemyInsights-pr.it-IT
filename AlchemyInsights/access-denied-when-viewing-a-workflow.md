---
title: Accesso negato durante la visualizzazione di un flusso di lavoro
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955205"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accesso negato durante la visualizzazione di un flusso di lavoro

SharePoint 2013 I flussi di lavoro che tentano di inviare un messaggio di posta elettronica a un gruppo di SharePoint possono avere esito negativo con un messaggio di errore "Accesso negato" se l'appartenenza al gruppo di SharePoint non è impostata su Tutti.
  
 **Per risolvere il problema, procedere come segue:**
  
 1. Consentire a tutti di visualizzare i membri del SharePoint gruppo.
  
 2. Rimuovere il SharePoint gruppo dalla riga A o CC del messaggio di posta elettronica.
  
 3. Aggiungi in modo esplicito gli utenti alla riga A o CC se non è possibile modificare la visibilità dell'appartenenza per SharePoint gruppo.
  
Per visualizzare ulteriori dettagli, fare riferimento a HTTP Non autorizzato [a /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  