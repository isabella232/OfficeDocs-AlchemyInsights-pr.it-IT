---
title: Il provisioning utente di Workday in AD va nello stato quarantena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430746"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="af4f2-102">Il provisioning utente di Workday in AD va nello stato quarantena</span><span class="sxs-lookup"><span data-stu-id="af4f2-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="af4f2-103">**Il provisioning utente di Workday in AD va nello stato quarantena e non viene creato alcun utente in AD**</span><span class="sxs-lookup"><span data-stu-id="af4f2-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="af4f2-104">Il provisioning utente di Workday in AD è andato in stato quarantena e i registri di controllo mostrano eventi di esportazioni non andate a buon fine con il messaggio di errore **Errore: OperationsError-SvcErr: si è verificato un errore nell'operazione. Non è stato configurato alcun riferimento superiore per il servizio directory. Il servizio directory non è quindi in grado di generare riferimenti a oggetti che si trovano all'esterno di questa foresta.**.</span><span class="sxs-lookup"><span data-stu-id="af4f2-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="af4f2-105">Questo errore in genere viene visualizzato se l'UO del contenitore di Active Directory non è impostata correttamente o se si sono verificati errori con il mapping espressione usato per **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="af4f2-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="af4f2-106">Controlla che l'UO predefinita per il parametro **Nuovi utenti** non contenga errori di digitazione.</span><span class="sxs-lookup"><span data-stu-id="af4f2-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="af4f2-107">Assicurati che l'UO specificata esista già in AD.</span><span class="sxs-lookup"><span data-stu-id="af4f2-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="af4f2-108">Se stai usando **parentDistinguishedName** nel mapping dell'attributo, assicurati che restituisca sempre un contenitore noto nel dominio AD.</span><span class="sxs-lookup"><span data-stu-id="af4f2-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="af4f2-109">Verifica Esporta evento nei registri di controllo per visualizzare il valore generato.</span><span class="sxs-lookup"><span data-stu-id="af4f2-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="af4f2-110">Per altri dettagli sulla configurazione di Workday per il provisioning automatizzato, consulta [Tutorial: configurare Workday per il provisioning utente automatico](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="af4f2-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

