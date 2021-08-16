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
ms.openlocfilehash: 24b9a7d3e8106c7357f14a00ecb192af4644257577a9549620b6e8b11b6f90d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097454"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Messaggio che informa che non è stato trovato alcun abbonamento nel Security Center

Se durante l'accesso a Microsoft Defender Security Center viene visualizzato il messaggio "Nessuna sottoscrizione trovata", l'istanza di Azure Active Directory (AAD) usata per consentire all'utente di accedere al portale non include una licenza di Microsoft Defender ATP.  

Le licenze di Windows E5 e Office E5 sono licenze distinte.

Aprire un caso di supporto se la licenza è stata acquistata ma non è stato eseguito il provisioning all'istanza di AAD. Potrebbe essersi verificato quanto segue: <br/>
-   Un possibile problema di provisioning della licenza.<br/>
-   È stato eseguito inavvertitamente il provisioning della licenza a un Microsoft AAD differente rispetto a quello usato per l'autenticazione al servizio.