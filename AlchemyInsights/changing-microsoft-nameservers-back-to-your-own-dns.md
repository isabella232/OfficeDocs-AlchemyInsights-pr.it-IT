---
title: Passaggio dai server dei nomi Microsoft alla gestione dei propri record DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481868"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Passaggio dai server dei nomi Microsoft alla gestione dei propri record DNS

In precedenza si sono modificati i record NS in modo che puntassero a Microsoft (ns1.bdm.microsoftonline.com) ma ora si è deciso di gestire i propri record DNS:

Nel sito Web del registrar, ripristinare il server dei nomi con il registrar o l'impostazione precedente. Se non si ha familiarità con il DNS, contattare il supporto del registrar. Tenere presente che la propagazione delle modifiche del server dei nomi può richiedere fino a 48 ore. 

1. Nel portale di amministrazione Microsoft 365, passare a **Impostazioni** > [**Domini**](https://admin.microsoft.com/Adminportal/Home#/Domains), selezionare la casella di controllo accanto al dominio e selezionare **Gestisci DNS**. 

2. Nella procedura guidata, selezionare **Aggiungere i propri record DNS** e completare la procedura. In questo modo viene modificata la modalità di gestione del DNS e quindi è possibile aggiungere i propri record DNS personalizzati necessari per supportare i servizi selezionati.

In alternativa, se i record dei server dei nomi sono stati modificati in Microsoft e si dispone di un sito Web, è possibile aggiungere record DNS per il sito Web anziché modificare di nuovo i server dei nomi. Per altre informazioni, vedere anche [Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


