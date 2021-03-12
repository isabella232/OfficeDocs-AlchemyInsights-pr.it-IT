---
title: Impossibile inviare/ricevere posta elettronica a/da Office 365 a causa della disabilitazione di TLS 1.0 e TLS 1.1
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
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726939"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Impossibile inviare/ricevere posta elettronica a/da Office 365 a causa della disabilitazione di TLS 1.0 e TLS 1.1

Come confermato dal post del centro messaggi MC229914, la deprecazione di TLS 1.0 e TLS 1.1 ha iniziato a far rispettare gli endpoint del flusso di posta di Exchange Online. Presto Office 365 non accetterà più le connessioni di posta elettronica TLS 1.0 e TLS 1.1 da origini esterne. Inoltre, Exchange Online non utilizzerà mai TLS 1.0 o 1.1 per inviare posta elettronica in uscita. Se si verificano problemi a causa della disabilitazione di TLS 1.0 o 1.1, è possibile che si verifichi uno dei seguenti errori:

- Il mittente riceve il mancato recapito del rapporto di mancato recapito - '421 4.4.2 Connessione interrotta a causa di SocketError'
- Errore nel Visualizzatore code del server locale che invia posta elettronica al responsabile 365- '421 4.4.2 Connessione interrotta a causa di SocketError'
- Errore nel registro del protocollo [del connettore di](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) invio sul server che invia la posta elettronica a Office 365- Negoziazione TLS non riuscita con errore SocketError
- Errore nel registro del protocollo del connettore di invio o ricezione - '451 5.7.3 Deve emettere prima un comando STARTTLS'

Se si verifica uno degli errori precedenti, assicurarsi che il server che sta inviando o ricevendo posta elettronica abbia TLS 1.2 abilitato controllando le seguenti chiavi del Registro di sistema:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Se si apportano modifiche alle chiavi del Registro di sistema precedenti per abilitare TLS 1.2, riavviare il server per rendere effettive le modifiche. Assicurarsi inoltre di avere installato gli aggiornamenti più recenti di Windows ed Exchange.

Per altre informazioni, vedere:

- [Exchange Server tls, parte 1: Getting Ready for TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server guida TLS Parte 2: abilitazione di TLS 1.2 e identificazione dei client che non lo usano - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Informazioni sugli scenari di posta elettronica se non è possibile concordare versioni TLS con Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
