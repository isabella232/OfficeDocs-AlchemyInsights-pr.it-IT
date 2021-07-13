---
title: Stato dominio - Nessun servizio selezionato
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389185"
---
# <a name="domain-status---no-services-selected"></a>Stato dominio - Nessun servizio selezionato

**Nessun servizio** selezionato significa che non hai selezionato alcun servizio Microsoft 365 come Exchange Online, Skype for Business o Intune e Gestione dispositivi mobili per Microsoft 365 da usare con il dominio personalizzato. Se si usa Exchange ibrido (Exchange locale con Exchange Online) o il filtro posta indesiderata esterno con Exchange e nessun altro servizi Microsoft, è possibile ignorare questo messaggio. Lo stato di integrità del dominio è disponibile solo per i domini connessi direttamente al servizio.

Per selezionare i servizi per il dominio:

1. Da **Impostazioni**, selezionare la casella accanto al dominio con  >  [](https://admin.microsoft.com/Adminportal/Home)il messaggio di stato Nessun **servizio selezionato.**
1. Selezionare **Gestisci DNS per** avviare l'Installazione guidata dominio.
    - Se si sceglie **Aggiungi record DNS personalizzati,** assicurarsi di selezionare un servizio quando richiesto. Altri servizi potrebbero essere disponibili in **Opzioni avanzate.**
    - Se si sceglie **Consenti a Microsoft di aggiungere** i record DNS o Altre opzioni Configura i miei servizi online per me tutti i servizi disponibili vengono suggeriti   >   e selezionati automaticamente.
1. Continuare con la procedura guidata per completare la configurazione DNS e le scelte del servizio.
 
Per ulteriori informazioni sulla configurazione del dominio, vedere [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

