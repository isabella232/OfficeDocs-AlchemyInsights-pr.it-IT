---
title: Utilizzo delle applicazioni iOS VPP regola ID 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558004"
---
# <a name="working-with-ios-vpp-applications"></a>Utilizzo delle applicazioni di iOS VPP

Leggere [come gestire le app iOS acquistate tramite un programma di acquisto di volumi con Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) per informazioni sulle caratteristiche, i vincoli e i passaggi necessari per utilizzare il programma di acquisto dei volumi di Apple e il relativo supporto in Microsoft Intune.
  
 **Problemi comuni:** "È stata assegnata un'app iOS VPP ai miei utenti, ma l'installazione ha avuto esito negativo".
  
- Questo può verificarsi se un singolo token VPP viene utilizzato su più provider di gestione dei dispositivi mobili. I token VPP di Apple possono essere utilizzati solo con un solo provider. Se è stato utilizzato un token VPP con più provider, è necessario caricare di nuovo il token in Intune.

- L'installazione può anche avere esito negativo se il numero totale di installazioni supera il numero di licenze. Per visualizzare un report di utilizzo per le licenze, accedere alla pagina **licenze app** per **dispositivi mobili** \> di Intune. Per informazioni su come recuperare le licenze in uso, vedere [questo articolo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
