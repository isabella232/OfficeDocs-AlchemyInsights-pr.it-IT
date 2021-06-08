---
title: Non è possibile attivare Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798684"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="e6184-102">Non è possibile attivare Office</span><span class="sxs-lookup"><span data-stu-id="e6184-102">Unable to activate Office</span></span>

<span data-ttu-id="e6184-103">**Nota**: se si sta usando una versione precedente di Windows (Ad esempio, Windows 7), assicurarsi che TLS 1.2 sia abilitato per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="e6184-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="e6184-104">Per ulteriori informazioni, vedere [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocollo di protezione predefinito in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="e6184-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="e6184-105">Verificare se lo stato dell'abbonamento risulti scaduto.</span><span class="sxs-lookup"><span data-stu-id="e6184-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="e6184-106">Assicurarsi di avere un abbonamento che consenta licenze client, ad esempio Office 365 Business o Business Premium, e [assicurarsi che all'utente sia assegnata una licenza](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="e6184-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="e6184-107">Assicurarsi che l'utente acceda a Office con lo stesso account a cui è assegnata la licenza.</span><span class="sxs-lookup"><span data-stu-id="e6184-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e6184-108">Controllare la [pagina sull'integrità dei servizi di Office 365](/office365/enterprise/view-service-health) per verificare se sono presenti problemi noti con il servizio.</span><span class="sxs-lookup"><span data-stu-id="e6184-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e6184-p102">Controllare le impostazioni del firewall, del software antivirus e del proxy per confermare che non stanno bloccando l'accesso delle app di Microsoft 365 a Internet. Vedere [URL e intervalli di indirizzi IP di Office 365](/office365/enterprise/urls-and-ip-address-ranges "Intervalli di indirizzi IP e URL di Office 365").</span><span class="sxs-lookup"><span data-stu-id="e6184-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="e6184-111">**Suggerimento:** nei computer Windows è possibile diagnosticare e risolvere automaticamente diversi problemi comuni di accesso a Office.</span><span class="sxs-lookup"><span data-stu-id="e6184-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="e6184-112">Scaricare ed eseguire l'**[Assistente supporto e ripristino di Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** per usare il tool automatizzato.</span><span class="sxs-lookup"><span data-stu-id="e6184-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="e6184-113">Utilizzare le seguenti opzioni di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="e6184-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="e6184-114">Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) dagli account utente esistenti.</span><span class="sxs-lookup"><span data-stu-id="e6184-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e6184-115">[Rimuovere](/microsoft-365/admin/manage/remove-licenses-from-users) e [riassegnare](/microsoft-365/admin/manage/assign-licenses-to-users) la licenza di Office, quindi [accedere a Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con l'account utente interessato.</span><span class="sxs-lookup"><span data-stu-id="e6184-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e6184-116">Eseguire lo [strumento di risoluzione dei problemi di attivazione.](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="e6184-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="e6184-117">Reimpostare lo stato di attivazione di Office</span><span class="sxs-lookup"><span data-stu-id="e6184-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reimpostare lo stato di attivazione di Office")
- [<span data-ttu-id="e6184-118">Eseguire un ripristino online di Office</span><span class="sxs-lookup"><span data-stu-id="e6184-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="e6184-119">Per ulteriori soluzioni per la risoluzione del problema, vedere:</span><span class="sxs-lookup"><span data-stu-id="e6184-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="e6184-120">Errori di attivazione e di tipo Prodotto senza licenza in Office</span><span class="sxs-lookup"><span data-stu-id="e6184-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="e6184-121">Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office</span><span class="sxs-lookup"><span data-stu-id="e6184-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)