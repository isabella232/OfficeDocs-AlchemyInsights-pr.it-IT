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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033282"
---
# <a name="configuring-the-provision-service"></a>Configurazione del servizio di provisioning

Per il funzionamento del provisioning automatico degli utenti, Azure AD richiede credenziali valide che gli consentano di connettersi all'API dei servizi Web Workday. Inoltre, il pulsante Test Connection nell'app Workday to AD User Provisioning verifica anche se è in grado di connettersi all'agente di provisioning di Azure AD Connessione associato al dominio AD.

Se il portale di Azure restituisce un errore al salvataggio delle credenziali, seguire i passaggi consigliati di seguito:

1. Verificare di aver configurato l'account utente del sistema di integrazione di Workday come indicato nella sezione dell'esercitazione Configurare l'utente del sistema di [integrazione in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Verificare che il servizio agente di provisioning di Azure AD Connessione sia in esecuzione nel server Windows locale tramite La console di gestione dei servizi. Puoi anche controllare lo stato dell'agente nel portale di Azure facendo clic sul pulsante Visualizza agenti locali.
3. Assicurati di immettere il valore per il campo "Nome utente workday" usando il formato username@workday-tenant-name. Se il workday-tenant-name è mancante, l'autenticazione workday ha esito negativo.
4. Se si sta configurando l'integrazione con il tenant di implementazione di Workday, prendere nota delle ore di inattività pianificate del tenant Workday. Workday ha pianificato il tempo di inattività per i tenant di implementazione durante i fine settimana (in genere dal venerdì sera al sabato mattina) e gli errori di connettività durante questa finestra di inattività sono un problema noto che si risolve automaticamente non appena i tenant di implementazione tornano online.
5. In rari casi, questo errore può essere visualizzato anche se la password dell'utente del sistema di integrazione è cambiata a causa dell'aggiornamento del tenant o se l'account è in stato bloccato o scaduto. Verificare lo stato dell'utente del sistema di integrazione con l'amministratore di Workday.

Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, vedere [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
