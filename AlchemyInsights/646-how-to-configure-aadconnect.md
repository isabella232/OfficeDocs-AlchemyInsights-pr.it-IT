---
title: 646 come configurare AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915581"
---
# <a name="configure-sync-features"></a>Configurare le funzionalità di sincronizzazione

Azure Active Directory Connetti includono diverse funzionalità che sono abilitati per impostazione predefinita o che è possibile abilitare più avanti. Alcune caratteristiche richiedono un'ulteriore configurazione in ambienti specifici.
  
- Limiti di [filtro](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) gli oggetti vengono sincronizzati con Azure Active Directory. Per impostazione predefinita, tutti gli utenti, contatti, gruppi e Windows 10 account computer sono sincronizzati. È possibile includere o escludere gli oggetti basati su domini, le unità organizzative o gli altri attributi. 
    
- [Sincronizzazione hash password](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Sincronizza il valore hash password da Active Directory locale per Azure Active Directory. In questo modo la gestione delle password in un'unica posizione, ma sfruttare la stessa password sia in locale e cloud ambienti. Dal momento che Active Directory è l'origine autorevole, è possibile utilizzare i proprio criteri password. 
    
- [Programma di reimpostazione password self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) consente agli utenti di reimpostare le password in cloud pur applicando i criteri password in locale. 
    
- [Dispositivo writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) consente ai dispositivi registrati in Azure Active Directory per essere scritto di Active Directory locale in modo che possono essere utilizzati per l'accesso condizionale. 
    
- [Impedisci accidentali Elimina](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) è abilitata per impostazione predefinita per evitare eliminazioni oggetto simultaneo troppi (più di 500 oggetti per la sincronizzazione). È possibile modificare questa impostazione per soddisfare le esigenze dell'organizzazione. 
    
- [Aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) è abilitata per impostazione predefinita per le installazioni express e consente di verificare che la versione della connessione di Azure Active Directory è sempre corrente. 
    

