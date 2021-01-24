---
title: Problema di provisioning con SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935379"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="b69f4-102">Problema di provisioning con SCIM</span><span class="sxs-lookup"><span data-stu-id="b69f4-102">SCIM provisioning issue</span></span>

<span data-ttu-id="b69f4-103">Per provisioning automatico si intende la creazione di identità utente e ruoli nelle applicazioni cloud a cui gli utenti hanno accesso.</span><span class="sxs-lookup"><span data-stu-id="b69f4-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="b69f4-104">Oltre a creare le identità utente, il provisioning automatico esegue la manutenzione e la rimozione delle identità utente quando cambiano lo stato o i ruoli.</span><span class="sxs-lookup"><span data-stu-id="b69f4-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="b69f4-105">Prima di iniziare una distribuzione, è possibile rivedere [Funzionamento del provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) per informazioni sul funzionamento del provisioning di Azure Active Directory (AD) e per suggerimenti per la configurazione.</span><span class="sxs-lookup"><span data-stu-id="b69f4-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="b69f4-106">Gli sviluppatori di applicazioni possono usare l'API di gestione utenti SCIM (System for Cross-Domain Identity Management) per abilitare il provisioning automatico di utenti e gruppi tra l'applicazione e Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b69f4-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="b69f4-107">L'articolo [Creazione di un endpoint SCIM e configurazione del provisioning degli utenti con Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) illustra come creare un endpoint SCIM e integrarlo con il servizio di provisioning di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b69f4-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



