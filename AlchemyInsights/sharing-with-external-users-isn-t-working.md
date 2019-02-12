---
title: Condivisione con utenti esterni non funziona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900877"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Correggere i problemi con la condivisione di contenuto di SharePoint con utenti esterni

Verificare che condivisione esterna è attivata per l'organizzazione:
  
1. Visitare il [servizi &amp; pagina di componenti aggiuntivi nell'interfaccia di amministrazione di Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), fare clic su **siti**.
    
2. Verificare che l'impostazione è attivata per "In". Se sono selezionati "Solo esistenti gli utenti esterni", verificare che l'utente esterno sia presente nell'interfaccia di amministrazione di Office 365.
    
Verificare che l'esterno condividerla attivato per il sito. Per una raccolta siti classica:
  
1. Nell'interfaccia di amministrazione SharePoint classica, nel riquadro sinistro fare clic su **raccolte siti**.
    
2. Selezionare uno o più siti e sulla barra multifunzione fare clic su **condivisione**.
    
Per un sito del team che appartiene a un gruppo di Office 365, o un sito di comunicazione:
  
- Questi nuovi tipi di sito hanno la stessa impostazione condivisione impostazione sul livello di organizzazione, a meno che l'impostazione del livello di organizzazione consente la condivisione file mediante collegamenti che non richiedono l'accesso. In questo caso, i siti di consentono la condivisione con nuovi ed esistenti gli utenti esterni che effettuano l'accesso. Per modificare l'impostazione per specifici siti, utilizzare la nuova interfaccia di amministrazione di SharePoint (anteprima) o PowerShell. [Ulteriori informazioni](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> L'impostazione della condivisione esterna per qualsiasi sito può essere più restrittivo dell'impostazione a livello di organizzazione, ma non più ampio di impostazione a livello di organizzazione. 
  

