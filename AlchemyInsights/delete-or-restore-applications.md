---
title: Eliminare o ripristinare applicazioni
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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102575"
---
# <a name="delete-or-restore-applications"></a>Eliminare o ripristinare applicazioni

**Per eliminare un'applicazione dal tenant di Azure AD:**

1. Nel portale **di Azure AD** selezionare Enterprise **applicazioni**. Individuare e selezionare l'applicazione che si desidera eliminare.
2. Nella sezione **Gestisci** del riquadro sinistro selezionare **Proprietà.**
3. Selezionare **Elimina** e quindi **Sì** per confermare che si desidera eliminare l'app dal tenant di Azure AD.

Per altre informazioni su come eliminare un'app, vedi Guida introduttiva: Eliminare un'applicazione dal [tenant di Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

In PowerShell, il cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rimuove le configurazioni del proxy di applicazione da un'applicazione specifica in Azure Active Directory e può eliminare completamente l'applicazione, se specificata.

È possibile **ripristinare un'applicazione eliminata** tramite PowerShell. Dopo aver identificato l'applicazione che si desidera ripristinare, è possibile ripristinarla [utilizzando Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
