---
title: Aggiunta di un sottodominio
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475984"
---
# <a name="adding-a-sub-domain"></a>Aggiunta di un sottodominio

I sottodomini possono essere aggiunti allo stesso tenant o a un tenant diverso rispetto al dominio padre. In entrambi i casi è necessario gestire le proprie impostazioni DNS nel sito Web del registrar. Se hai lasciato a Microsoft la gestione delle impostazioni DNS con i record NS o se hai acquistato il dominio da Microsoft, non puoi aggiungere sottodomini senza prima modificare questa impostazione.

Aggiungere prima il dominio padre e quindi il sottodominio. Se il sottodominio si trova nello stesso tenant, non è necessaria alcuna verifica aggiuntiva. Se si aggiunge il sottodominio a un tenant separato, il record txt DNS è necessario per la verifica della proprietà prima di aggiungere il dominio e i record DNS aggiuntivi per i servizi selezionati.

- Per aggiungere un dominio o un sottodominio, seguire la procedura guidata Aggiungi dominio [oppure](https://admin.microsoft.com/Adminportal#/Domains/Wizard)aggiungere manualmente il dominio o il sottodominio andando a **Impostazione**  >  **domini**  >  **Aggiungi dominio**.

Se necessario:

- Per modificare chi gestisce le impostazioni DNS per un dominio esistente, passare **a Impostazioni**  >  [**Domains,**](https://admin.microsoft.com/Adminportal/Home#/Domains)selezionare la casella di controllo accanto al dominio e quindi **selezionare Manage DNS**. Nella procedura guidata, selezionare **Aggiungi i propri record DNS** e completare la procedura guidata.
- Per aggiungere sottodomini a un dominio acquistato da Microsoft, trasferire prima il dominio a un altro registrar e quindi apportare la modifica precedente per gestire i propri record DNS. Per istruzioni, vedere [Trasferire un dominio da Microsoft a un altro host.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Se viene visualizzato un messaggio di errore che indica che il dominio è già in uso da altri membri o persone dell'organizzazione, sarà innanzitutto necessario assumere questo account non gestito prima di utilizzare il dominio. Per istruzioni, vedere [Assumere una directory non gestita come amministratore in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
