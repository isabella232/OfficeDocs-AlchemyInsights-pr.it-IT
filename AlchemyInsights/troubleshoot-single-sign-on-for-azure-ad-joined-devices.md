---
title: "Risolvere i problemi relativi all'accesso Single #A0 per i dispositivi aggiunti ad Azure AD"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898083"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="c3876-102">Risolvere i problemi relativi all'accesso Single #A0 per i dispositivi aggiunti ad Azure AD</span><span class="sxs-lookup"><span data-stu-id="c3876-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="c3876-103">Se si dispone di un ambiente Active Directory (AD) locale e si desidera aggiungere i computer aggiunti al dominio DI AD ad Azure AD, è possibile eseguire questa operazione eseguendo l'aggiunta ibrida di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c3876-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="c3876-104">[Procedura: Pianificare l'implementazione ibrida](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dell'aggiunta ad Azure Active Directory fornisce i passaggi correlati per implementare un'aggiunta ibrida di Azure AD nell'ambiente.</span><span class="sxs-lookup"><span data-stu-id="c3876-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="c3876-105">Per ulteriori informazioni, vedere [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="c3876-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="c3876-106">**Problemi relativi al token di aggiornamento primario**</span><span class="sxs-lookup"><span data-stu-id="c3876-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="c3876-107">Un token di aggiornamento primario (PRT) è un elemento chiave dell'autenticazione di Azure AD nei dispositivi Windows 10, Windows Server 2016 e versioni successive, iOS e Android.</span><span class="sxs-lookup"><span data-stu-id="c3876-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="c3876-108">Si tratta di un token Web JSON (JWT) rilasciato appositamente ai broker di token di prima parte Microsoft per abilitare single sign-on (SSO) tra le applicazioni usate in tali dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c3876-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="c3876-109">Per informazioni dettagliate su come viene emesso, usato e protetto un PRT nei dispositivi Windows 10, vedi Che [cos'è un token di aggiornamento primario?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="c3876-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="c3876-110">**WamDefaultSet: SÌ e AzureADPrt: SÌ**</span><span class="sxs-lookup"><span data-stu-id="c3876-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="c3876-111">Questi campi indicano se l'utente ha eseguito correttamente l'autenticazione in Azure AD durante l'accesso al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3876-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="c3876-112">Se i valori sono **NO**, potrebbe essere dovuto a:</span><span class="sxs-lookup"><span data-stu-id="c3876-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="c3876-113">Chiave di archiviazione non compatibile nel TPM associato al dispositivo al momento della registrazione (controllare KeySignTest durante l'esecuzione con privilegi elevati)</span><span class="sxs-lookup"><span data-stu-id="c3876-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="c3876-114">ID di accesso alternativo</span><span class="sxs-lookup"><span data-stu-id="c3876-114">Alternate Login ID</span></span>
- <span data-ttu-id="c3876-115">Proxy HTTP non trovato</span><span class="sxs-lookup"><span data-stu-id="c3876-115">HTTP Proxy not found</span></span>

<span data-ttu-id="c3876-116">Per risolvere i problemi relativi ai dispositivi tramite il comando dsregcmd, vedere [Stato SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="c3876-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
