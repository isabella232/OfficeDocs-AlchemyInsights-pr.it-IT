---
title: 646 come configurare AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295977"
---
# <a name="configure-sync-features"></a><span data-ttu-id="bffa4-102">Configurare le funzionalità di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="bffa4-102">Configure sync features</span></span>

<span data-ttu-id="bffa4-p101">Azure Active Directory Connetti includono diverse funzionalità che sono abilitati per impostazione predefinita o che è possibile abilitare più avanti. Alcune caratteristiche richiedono un'ulteriore configurazione in ambienti specifici.</span><span class="sxs-lookup"><span data-stu-id="bffa4-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="bffa4-p102">Limiti di [filtro](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) gli oggetti vengono sincronizzati con Azure Active Directory. Per impostazione predefinita, tutti gli utenti, contatti, gruppi e Windows 10 account computer sono sincronizzati. È possibile includere o escludere gli oggetti basati su domini, le unità organizzative o gli altri attributi.</span><span class="sxs-lookup"><span data-stu-id="bffa4-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="bffa4-p103">[Sincronizzazione hash password](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Sincronizza il valore hash password da Active Directory locale per Azure Active Directory. In questo modo la gestione delle password in un'unica posizione, ma sfruttare la stessa password sia in locale e cloud ambienti. Dal momento che Active Directory è l'origine autorevole, è possibile utilizzare i proprio criteri password.</span><span class="sxs-lookup"><span data-stu-id="bffa4-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="bffa4-111">[Programma di reimpostazione password self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) consente agli utenti di reimpostare le password in cloud pur applicando i criteri password in locale.</span><span class="sxs-lookup"><span data-stu-id="bffa4-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="bffa4-112">[Dispositivo writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) consente ai dispositivi registrati in Azure Active Directory per essere scritto di Active Directory locale in modo che possono essere utilizzati per l'accesso condizionale.</span><span class="sxs-lookup"><span data-stu-id="bffa4-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="bffa4-p104">[Impedisci accidentali Elimina](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) è abilitata per impostazione predefinita per evitare eliminazioni oggetto simultaneo troppi (più di 500 oggetti per la sincronizzazione). È possibile modificare questa impostazione per soddisfare le esigenze dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="bffa4-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="bffa4-115">[Aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) è abilitata per impostazione predefinita per le installazioni express e consente di verificare che la versione della connessione di Azure Active Directory è sempre corrente.</span><span class="sxs-lookup"><span data-stu-id="bffa4-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

