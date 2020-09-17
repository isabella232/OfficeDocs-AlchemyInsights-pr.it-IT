---
title: Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815789"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting

1. Nell'interfaccia di amministrazione di Microsoft 365 passare alla pagina **installazione**  >  [domini](https://admin.microsoft.com/Adminportal#/Domains) e nell'elenco dei domini selezionare il dominio che si sta utilizzando per il sito Web.

2. Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:

  - Per **Tipo di DNS** immettere: **A (Indirizzo)**

  - Per **Nome host o alias** digitare **@**

  - Per **Indirizzo IP** digitare l'indirizzo IP presso cui il sito Web è attualmente ospitato, ad esempio 172.16.140.1.

    Deve essere un indirizzo IP  *statico*  , non  *dinamico*  , per il sito Web. Contattare il provider in cui è ospitato il sito Web per verificare che sia possibile ottenere un indirizzo IP statico per il sito Web pubblico.

3. Selezionare **Salva**.

È anche possibile creare un record CNAME per aiutare i clienti a trovare il sito Web.
  
1. Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:

  - Per **Tipo di DNS** immettere: **CNAME (Alias)**

  - Per **Nome host o alias** digitare **www**

  - Per **Indirizzo di puntamento** digitare il nome di dominio completo (FQDN) del sito Web, ad esempio contoso.com).

2. Selezionare **Salva**.
