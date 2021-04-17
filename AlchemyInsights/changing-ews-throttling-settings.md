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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818040"
---
# <a name="changing-ews-throttling-settings"></a>Modificare le impostazioni della limitazione EWS

Eseguire il test automatico che consente di modificare i criteri di limitazione EWS per la durata della migrazione. Tenere presente che, anche dopo l'esecuzione, le importazioni di EWS saranno comunque limitate a 150 MB ogni 5 minuti per cassetta postale. Per ottenere velocità di migrazione più elevate, eseguire simultaneamente la migrazione di più utenti.

Si prega di notare che le modifiche apportate ai criteri di limitazione EWS non hanno alcun effetto sui seguenti tipi di trasferimenti (in caso di utilizzo di strumenti Microsoft): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Cartelle Pubbliche o il Servizio d’importazione PST.