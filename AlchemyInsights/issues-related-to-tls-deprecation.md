---
title: Impossibile inviare/ricevere posta elettronica a/da Office 365 a causa della disabilitazione di TLS 1.0 e TLS 1.1
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
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726939"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="5d586-102">Impossibile inviare/ricevere posta elettronica a/da Office 365 a causa della disabilitazione di TLS 1.0 e TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="5d586-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="5d586-103">Come confermato dal post del centro messaggi MC229914, la deprecazione di TLS 1.0 e TLS 1.1 ha iniziato a far rispettare gli endpoint del flusso di posta di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5d586-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="5d586-104">Presto Office 365 non accetterà più le connessioni di posta elettronica TLS 1.0 e TLS 1.1 da origini esterne.</span><span class="sxs-lookup"><span data-stu-id="5d586-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="5d586-105">Inoltre, Exchange Online non utilizzerà mai TLS 1.0 o 1.1 per inviare posta elettronica in uscita.</span><span class="sxs-lookup"><span data-stu-id="5d586-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="5d586-106">Se si verificano problemi a causa della disabilitazione di TLS 1.0 o 1.1, è possibile che si verifichi uno dei seguenti errori:</span><span class="sxs-lookup"><span data-stu-id="5d586-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="5d586-107">Il mittente riceve il mancato recapito del rapporto di mancato recapito - '421 4.4.2 Connessione interrotta a causa di SocketError'</span><span class="sxs-lookup"><span data-stu-id="5d586-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="5d586-108">Errore nel Visualizzatore code del server locale che invia posta elettronica al responsabile 365- '421 4.4.2 Connessione interrotta a causa di SocketError'</span><span class="sxs-lookup"><span data-stu-id="5d586-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="5d586-109">Errore nel registro del protocollo [del connettore di](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) invio sul server che invia la posta elettronica a Office 365- Negoziazione TLS non riuscita con errore SocketError</span><span class="sxs-lookup"><span data-stu-id="5d586-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="5d586-110">Errore nel registro del protocollo del connettore di invio o ricezione - '451 5.7.3 Deve emettere prima un comando STARTTLS'</span><span class="sxs-lookup"><span data-stu-id="5d586-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="5d586-111">Se si verifica uno degli errori precedenti, assicurarsi che il server che sta inviando o ricevendo posta elettronica abbia TLS 1.2 abilitato controllando le seguenti chiavi del Registro di sistema:</span><span class="sxs-lookup"><span data-stu-id="5d586-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="5d586-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="5d586-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="5d586-113">Se si apportano modifiche alle chiavi del Registro di sistema precedenti per abilitare TLS 1.2, riavviare il server per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="5d586-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="5d586-114">Assicurarsi inoltre di avere installato gli aggiornamenti più recenti di Windows ed Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d586-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="5d586-115">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="5d586-115">For more information, see:</span></span>

- [<span data-ttu-id="5d586-116">Exchange Server tls, parte 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="5d586-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="5d586-117">Exchange Server guida TLS Parte 2: abilitazione di TLS 1.2 e identificazione dei client che non lo usano - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="5d586-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="5d586-118">Informazioni sugli scenari di posta elettronica se non è possibile concordare versioni TLS con Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="5d586-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
