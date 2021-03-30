---
title: Single-Sign per i dispositivi aggiunti ad Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403828"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="c428c-102">Single #A0 per i dispositivi aggiunti ad Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c428c-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="c428c-103">Se si dispone di un ambiente Active Directory (AD) locale e si desidera aggiungere i computer aggiunti al dominio DI AD ad Azure AD, è possibile eseguire questa operazione eseguendo l'aggiunta ibrida di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c428c-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="c428c-104">[Procedura: Pianificare l'implementazione ibrida](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dell'aggiunta ad Azure Active Directory fornisce i passaggi correlati per implementare un'aggiunta ibrida di Azure AD nell'ambiente.</span><span class="sxs-lookup"><span data-stu-id="c428c-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="c428c-105">Configurare i dispositivi aggiunti ad Azure AD per i dispositivi locali Single-Sign l'uso di Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="c428c-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="c428c-106">**Problemi relativi al token di aggiornamento primario** Un token di aggiornamento primario (PRT) è un elemento chiave dell'autenticazione di Azure AD nei dispositivi Windows 10, Windows Server 2016 e versioni successive, iOS e Android.</span><span class="sxs-lookup"><span data-stu-id="c428c-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="c428c-107">Si tratta di un token Web JSON (JWT) rilasciato appositamente ai broker di token di prima parte Microsoft per abilitare single sign-on (SSO) tra le applicazioni usate in tali dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c428c-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="c428c-108">[In Che cos'è un token](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)di aggiornamento primario? , forniremo informazioni dettagliate su come viene emesso, usato e protetto un PRT nei dispositivi Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c428c-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="c428c-109">**WamDefaultSet: SÌ e AzureADPrt: SÌ** Questi campi indicano se l'utente ha eseguito correttamente l'autenticazione in Azure AD durante l'accesso al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c428c-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="c428c-110">Se i valori sono **NO,** potrebbe essere dovuto:</span><span class="sxs-lookup"><span data-stu-id="c428c-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="c428c-111">Chiave di archiviazione non disponibile nel TPM associato al dispositivo al momento della registrazione (controllare KeySignTest durante l'esecuzione con privilegi elevati).</span><span class="sxs-lookup"><span data-stu-id="c428c-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="c428c-112">ID di accesso alternativo</span><span class="sxs-lookup"><span data-stu-id="c428c-112">Alternate Login ID</span></span>
- <span data-ttu-id="c428c-113">Proxy HTTP non trovato</span><span class="sxs-lookup"><span data-stu-id="c428c-113">HTTP Proxy not found</span></span>

<span data-ttu-id="c428c-114">Risolvere i problemi relativi ai dispositivi tramite il comando dsregcmd - [Stato SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="c428c-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
