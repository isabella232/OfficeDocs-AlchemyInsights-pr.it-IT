---
title: La condivisione con utenti esterni non funziona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304373"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Risolvere i problemi di condivisione SharePoint contenuto con utenti esterni

Verificare che la condivisione esterna sia attivata per l'organizzazione:
  
1. Passare alla [pagina Componenti aggiuntivi servizi &amp; nell'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e fare clic su **Siti**.
    
2. Assicurati che l'impostazione sia attivata. Se è selezionata l'opzione "Solo utenti esterni esistenti", verificare che l'utente esterno sia elencato nella interfaccia di amministrazione di Microsoft 365.
    
Verificare che la condivisione esterna sia attivata per il sito. Per una raccolta siti classica:
  
1. Nel nuovo SharePoint di amministrazione fare clic su siti nel riquadro **sinistro.**
    
2. Selezionare il sito o i siti e sulla barra multifunzione fare clic su **Condivisione.**
    
Per un sito del team appartenente a un Microsoft 365 o a un sito di comunicazione:
  
- Questi nuovi tipi di siti hanno la stessa impostazione di condivisione dell'organizzazione, a meno che l'impostazione a livello di organizzazione non consenta la condivisione di file utilizzando collegamenti che non richiedono l'accesso. In questo caso, i siti consentono la condivisione con utenti esterni nuovi ed esistenti che effettuano l'accesso. Per modificare l'impostazione per siti specifici, usare la nuova interfaccia SharePoint o PowerShell. [Altre informazioni](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Nota:** l'impostazione di condivisione esterna per qualsiasi sito può essere più restrittiva rispetto all'impostazione a livello di organizzazione, ma non più permissiva rispetto all'impostazione a livello di organizzazione. 
  

