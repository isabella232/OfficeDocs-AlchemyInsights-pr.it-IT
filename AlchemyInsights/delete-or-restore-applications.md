---
title: Eliminare o ripristinare le applicazioni
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013958"
---
# <a name="delete-or-restore-applications"></a>Eliminare o ripristinare le applicazioni

**Per eliminare un'applicazione dal tenant di Azure ad**:

1. Nel **portale di Azure ad**, selezionare **applicazioni Enterprise**. Quindi individuare e selezionare l'applicazione che si desidera eliminare.
2. Nella sezione **Gestisci** del riquadro sinistro selezionare **Proprietà**.
3. Selezionare **Elimina**, quindi fare clic su **Sì** per confermare che si desidera eliminare l'app dal tenant di Azure ad.

Per ulteriori informazioni su come eliminare un'app, vedere [Guida introduttiva: eliminare un'applicazione dal tenant di Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

In PowerShell, il cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rimuove le configurazioni del proxy di applicazione da un'applicazione specifica in Azure Active Directory ed è in grado di eliminare completamente l'applicazione, se specificata.

È possibile **ripristinare un'applicazione eliminata** tramite PowerShell. Dopo che l'applicazione che si desidera ripristinare è stata identificata, è possibile ripristinarla utilizzando [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
