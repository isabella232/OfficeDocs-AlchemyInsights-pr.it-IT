---
title: Configurazione del servizio di provisioning
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480750"
---
# <a name="configuring-the-provision-service"></a>Configurazione del servizio di provisioning

Per il funzionamento del provisioning automatico degli utenti, Azure AD richiede credenziali valide che gli consentono di connettersi all'API dei servizi Web Workday. Inoltre, il pulsante Test Connection nell'app Workday to AD User Provisioning verifica anche se è in grado di connettersi all'agente di provisioning di Azure AD Connect associato al dominio AD.

Se il portale di Azure restituisce un errore al salvataggio delle credenziali, seguire i passaggi consigliati di seguito:

1. Verificare di aver configurato l'account utente del sistema di integrazione Workday come indicato nella sezione relativa all'esercitazione Configurare l'utente del sistema di [integrazione in Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Verificare che il servizio agente di provisioning di Azure AD Connect sia operativo nel server Windows locale tramite la console di gestione dei servizi. È anche possibile controllare lo stato dell'agente nel portale di Azure facendo clic sul pulsante Visualizza agenti locali.
3. Assicurarsi di immettere il valore del campo "Nome utente workday" utilizzando il formato username@workday-tenant-name. Se il workday-tenant-name non è presente, l'autenticazione di Workday ha esito negativo.
4. Se si sta configurando l'integrazione con il tenant di implementazione di Workday, prendere nota delle ore di inattività pianificate del tenant di Workday. Workday ha pianificato il tempo di inattività per i tenant di implementazione nei fine settimana (in genere dal venerdì sera al sabato mattina) e gli errori di connettività durante questo periodo di inattività sono un problema noto che si risolve automaticamente non appena i tenant di implementazione sono di nuovo online.
5. In rari casi, questo errore può essere visualizzato anche se la password dell'utente del sistema di integrazione è cambiata a causa dell'aggiornamento del tenant o se l'account è in stato bloccato o scaduto. Verificare lo stato dell'utente del sistema di integrazione con l'amministratore di Workday.

Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, consulta [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
