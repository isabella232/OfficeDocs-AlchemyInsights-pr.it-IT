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
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779516"
---
# <a name="configure-sync-features"></a><span data-ttu-id="9fd17-102">Configurare le funzionalità di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="9fd17-102">Configure sync features</span></span>

<span data-ttu-id="9fd17-103">Azure AD Connect include diverse funzionalità che sono abilitate per impostazione predefinita o che possono essere abilitate in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="9fd17-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="9fd17-104">Alcune funzionalità richiedono una configurazione aggiuntiva in ambienti specifici.</span><span class="sxs-lookup"><span data-stu-id="9fd17-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="9fd17-105">Limiti del [filtro](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) gli oggetti vengono sincronizzati con Azure ad.</span><span class="sxs-lookup"><span data-stu-id="9fd17-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="9fd17-106">Per impostazione predefinita, tutti gli utenti, i contatti, i gruppi e gli account computer di Windows 10 sono sincronizzati.</span><span class="sxs-lookup"><span data-stu-id="9fd17-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="9fd17-107">È possibile includere o escludere oggetti basati su domini, unità organizzative o altri attributi.</span><span class="sxs-lookup"><span data-stu-id="9fd17-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="9fd17-108">[Password hash sincronizzazione](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizza l'hash della password da Active Directory locale AD Azure ad.</span><span class="sxs-lookup"><span data-stu-id="9fd17-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="9fd17-109">In questo modo la gestione delle password viene consentita in una posizione, ma viene utilizzata la stessa password sia in ambienti locali che in quelli cloud.</span><span class="sxs-lookup"><span data-stu-id="9fd17-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="9fd17-110">Poiché Active Directory è l'origine autorevole, è possibile utilizzare i criteri di password personalizzati.</span><span class="sxs-lookup"><span data-stu-id="9fd17-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="9fd17-111">La reimpostazione della [password in modalità self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) consente agli utenti di reimpostare le proprie password nel cloud pur applicando i criteri di password locali.</span><span class="sxs-lookup"><span data-stu-id="9fd17-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="9fd17-112">Il [writeback del dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) consente ai dispositivi registrati in Azure ad di essere riScritti in Active Directory locale in modo che possano essere utilizzati per l'accesso condizionale.</span><span class="sxs-lookup"><span data-stu-id="9fd17-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="9fd17-113">[Impedisci eliminazioni accidentali](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) è abilitata per impostazione predefinita per evitare troppe eliminazioni simultanee degli oggetti (più di 500 Object per sincronizzazione).</span><span class="sxs-lookup"><span data-stu-id="9fd17-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="9fd17-114">È possibile modificare questa impostazione in modo da soddisfare le esigenze dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="9fd17-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="9fd17-115">L' [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) è abilitato per impostazione predefinita per le installazioni Express e garantisce che la versione di Azure ad Connect sia sempre aggiornata.</span><span class="sxs-lookup"><span data-stu-id="9fd17-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

