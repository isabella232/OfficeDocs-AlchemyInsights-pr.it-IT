---
title: Writeback dei dispositivi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255171"
---
# <a name="device-writeback"></a><span data-ttu-id="60fa6-102">Writeback dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="60fa6-102">Device Writeback</span></span>

<span data-ttu-id="60fa6-103">Il writeback dei dispositivi viene utilizzato negli scenari seguenti:</span><span class="sxs-lookup"><span data-stu-id="60fa6-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="60fa6-104">Abilitare [Windows Hello for Business con la distribuzione trust certificato ibrida](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="60fa6-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="60fa6-105">Abilitare l'accesso condizionale in base ai dispositivi alle applicazioni protette di ADFS (2012 R2 o versione successiva) (attendibilità relying party)</span><span class="sxs-lookup"><span data-stu-id="60fa6-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="60fa6-106">È necessaria una sottoscrizione ad Azure AD Premium per il writeback del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60fa6-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="60fa6-107">In questo modo si garantisce una sicurezza e una garanzia aggiuntive che l'accesso alle applicazioni viene concesso solo ai dispositivi attendibili.</span><span class="sxs-lookup"><span data-stu-id="60fa6-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="60fa6-108">Per ulteriori informazioni sull'accesso condizionale, vedere [Gestione](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) dei rischi con l'accesso condizionale e Configurazione dell'accesso condizionale locale tramite la registrazione dei dispositivi [di Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="60fa6-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="60fa6-109">Per altre informazioni sull'abilitazione del writeback dei dispositivi per i dispositivi, vedi [Abilitare il writeback dei dispositivi.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="60fa6-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
