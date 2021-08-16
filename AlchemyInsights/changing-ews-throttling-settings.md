---
title: Modificare le impostazioni della limitazione EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968381"
---
# <a name="changing-ews-throttling-settings"></a>Modificare le impostazioni della limitazione EWS

Eseguire il test automatico che consente di modificare i criteri di limitazione EWS per la durata della migrazione. Tenere presente che, anche dopo l'esecuzione, le importazioni di EWS saranno comunque limitate a 150 MB ogni 5 minuti per cassetta postale. Per ottenere velocità di migrazione più elevate, eseguire simultaneamente la migrazione di più utenti.

Si prega di notare che le modifiche apportate ai criteri di limitazione EWS non hanno alcun effetto sui seguenti tipi di trasferimenti (in caso di utilizzo di strumenti Microsoft): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Cartelle Pubbliche o il Servizio d’importazione PST.