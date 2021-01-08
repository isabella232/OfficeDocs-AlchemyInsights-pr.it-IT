---
title: Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768526"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center

Se durante l'accesso al Microsoft Defender Security Center viene visualizzato il messaggio "Non è stato trovato alcun abbonamento", significa che Azure Active Directory (AAD) usato per far accedere l'utente al portale non dispone di una licenza di Microsoft Defender ATP.  

Le licenze di Windows E5 e Office E5 sono licenze distinte.

Aprire un caso di supporto se la licenza è stata acquistata ma non è stato eseguito il provisioning all'istanza di AAD. Potrebbe essersi verificato quanto segue: <br/>
-   Un possibile problema di provisioning della licenza.<br/>
-   È stato eseguito inavvertitamente il provisioning della licenza a un Microsoft AAD differente rispetto a quello usato per l'autenticazione al servizio.