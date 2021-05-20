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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544112"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center

Se durante l'accesso a Microsoft Defender Security Center viene visualizzato il messaggio "Nessuna sottoscrizione trovata", l'istanza di Azure Active Directory (AAD) usata per consentire all'utente di accedere al portale non include una licenza di Microsoft Defender ATP.  

Le licenze di Windows E5 e Office E5 sono licenze distinte.

Aprire un caso di supporto se la licenza è stata acquistata ma non è stato eseguito il provisioning all'istanza di AAD. Potrebbe essersi verificato quanto segue: <br/>
-   Un possibile problema di provisioning della licenza.<br/>
-   È stato eseguito inavvertitamente il provisioning della licenza a un Microsoft AAD differente rispetto a quello usato per l'autenticazione al servizio.