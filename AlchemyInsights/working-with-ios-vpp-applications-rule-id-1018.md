---
title: Utilizzo di iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083018"
---
# <a name="working-with-ios-vpp-applications"></a>Utilizzo delle applicazioni VPP iOS

Leggi Come gestire le app [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) acquistate tramite un programma di acquisto di contratti multilicenza con Microsoft Intune per informazioni su funzionalità, vincoli e passaggi per usare il Programma di acquisto di contratti multilicenza Apple e il supporto per questo programma in Microsoft Intune.
  
 **Problemi comuni:** "Ho assegnato un'app VPP iOS agli utenti, ma l'installazione non è riuscita."
  
- Ciò può verificarsi se viene usato un singolo token VPP tra più provider di gestione dei dispositivi mobili. I token VPP di Apple possono essere usati solo con un provider. Se hai usato un token VPP con più provider, devi ricaricare il token in Intune.

- L'installazione può avere esito negativo anche se il numero totale di installazioni supera il numero di licenze. Per visualizzare un report di utilizzo per le licenze, passare alla pagina Licenze **app app intune per dispositivi** \>  mobili. Per informazioni su come recuperare le licenze in uso, vedi [questo articolo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
