---
title: Utilizzo di iOS VPP applicazioni regola Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296860"
---
# <a name="working-with-ios-vpp-applications"></a>Utilizzo di iOS VPP applicazioni

Informazioni su [come gestire le app di iOS acquistato tramite un programma volume di acquisto con Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) informazioni sulle caratteristiche, vincoli e operazioni affinché utilizzare del programma di acquisto Volume Apple e il relativo supporto Microsoft Intune. 
  
 **Problemi comuni:** "Un'app di iOS VPP sono stati assegnati agli utenti, ma l'installazione non riuscita" 
  
- Ciò può verificarsi se viene utilizzato un singolo token VPP tra più provider di gestione di dispositivi mobili. I token VPP Apple possono essere utilizzati solo con un provider. Se è stato utilizzato un token VPP con più provider, è necessario caricare nuovamente il token da Intune.
    
- L'installazione di esito negativo anche se il numero totale di installazioni supera il numero di licenze. Per visualizzare un report di utilizzo per le licenze, passare a **Intune Mobile App** \> pagina **licenze per l'applicazione** . Per informazioni su come liberare le licenze in uso, vedere [in questo articolo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

