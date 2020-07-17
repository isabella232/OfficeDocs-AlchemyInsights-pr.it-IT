---
title: Problemi con la licenza di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146810"
---
# <a name="yammer-licensing-issues"></a>Problemi con la licenza di Yammer

Tutti gli utenti devono disporre di una licenza per usare il servizio Yammer Enterprise, ma per impostazione predefinita, Yammer non richiede che gli utenti abbiano una licenza per accedere al servizio. Quando un amministratore modifica l'impostazione per bloccare gli utenti di Microsoft 365 senza licenza di Yammer, gli utenti a cui non sia stata assegnata una licenza di Yammer Enterprise non possono accedere al servizio Yammer. Per ulteriori informazioni, vedere [Gestire le licenze utente di Yammer in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Quando le licenze vengono rimosse dagli utenti, il riquadro Yammer non viene più visualizzato e altri servizi possono usare la rimozione della licenza per nascondere le funzionalità. In altri casi, le funzionalità possono comunque essere visualizzate, ma è necessario assegnare delle licenze per poterle utilizzare.  

**La licenza non viene aggiornata per l'utente**  

A volte, a un utente è assegnata una licenza, ma non è ancora possibile accedere a Yammer. È più probabile che si verifichino ritardi quando è in corso un'assegnazione di licenza in blocco. Gli utenti di Yammer potrebbero non essere aggiornati nello stesso ordine in cui le licenze sono state modificate in Azure AD perché il sistema viene eseguito in modo asincrono. Attendere fino a 24 ore prima di aprire un caso di supporto per segnalare i problemi di sincronizzazione della licenza.  

**Assegnazione di licenze in blocco**  

È possibile assegnare licenze tramite l'interfaccia di amministrazione o gli script di PowerShell. Per altre informazioni, vedere [Assegnare licenze agli utenti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e [Assegnare licenze agli account utente con Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Il supporto Microsoft non offre assistenza per la creazione di script, ma è disponibile la documentazione sull'assegnazione di licenze di Yammer. Per altre informazioni, vedere [Gestire le licenze di Yammer usando Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).