---
title: Configurare il servizio MIM Sync
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430741"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="79b43-102">Configurare il servizio MIM Sync</span><span class="sxs-lookup"><span data-stu-id="79b43-102">Configure MIM Sync service</span></span>

<span data-ttu-id="79b43-103">Il servizio di sincronizzazione Microsoft Identity Manager (MIM) è un componente di MIM.</span><span class="sxs-lookup"><span data-stu-id="79b43-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="79b43-104">Si tratta di un servizio centralizzato locale che archivia e integra le informazioni per le organizzazioni che dispongono di più directory e database locali.</span><span class="sxs-lookup"><span data-stu-id="79b43-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="79b43-105">Potrebbe essere possibile risolvere il problema con MIM Sync qualora fosse stato risolto da un aggiornamento recente di MIM o fosse tra i problemi menzionati nella sezione che segue.</span><span class="sxs-lookup"><span data-stu-id="79b43-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="79b43-106">**Passaggi consigliati**</span><span class="sxs-lookup"><span data-stu-id="79b43-106">**Recommended steps**</span></span>

1. <span data-ttu-id="79b43-107">Assicurati di usare un aggiornamento recente di MIM Sync e controlla le [note sulla versione di MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) per scoprire se il problema è stato risolto in un aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="79b43-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="79b43-108">Se il problema si riferisce a LDAP generico, SQL generico, Lotus Domino o a un connettore ai servizi Web, assicurati di usare un aggiornamento recente dei [connettori generici](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="79b43-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="79b43-109">Se un'esecuzione di MIM Sync si interrompe con un errore, consulta la tabella dei [codici di errore](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) per determinarne le cause potenziali.</span><span class="sxs-lookup"><span data-stu-id="79b43-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="79b43-110">Se l'esecuzione viene interrotta con **extension-dll-exception**, fai clic su queste parole per aprire la finestra delle **proprietà dell'oggetto spazio connettore** e fai clic su **Analisi dello stack...** per visualizzare altre informazioni sulla causa sottostante, come descritto in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="79b43-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="79b43-111">Se il componente Password Change Notification Service (PCNS) riporta l'**errore 6025** nel registro eventi durante la sincronizzazione della password, consulta la guida per la risoluzione dei problemi [PCNS segnala errore 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="79b43-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="79b43-112">Se la sincronizzazione completa con l'agente di gestione del servizio FIM fosse lenta, controllare l'impostazione **espansione automatica** per TempDB, come descritto in [Risoluzione dei problemi in caso la sincronizzazione completa sia lenta o venga sospesa](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="79b43-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="79b43-113">In caso riscontrassi un errore stopped-server con failed-creation-via-web-services durante l'utilizzo dell'agente di gestione del servizio FIM, consulta [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) per una panoramica delle cause.</span><span class="sxs-lookup"><span data-stu-id="79b43-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

