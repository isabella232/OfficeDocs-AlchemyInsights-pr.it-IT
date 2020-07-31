---
title: Risoluzione dei problemi relativi alla distribuzione del certificato di autenticazione client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509072"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="3a1e4-102">Risoluzione dei problemi relativi alla distribuzione del certificato di autenticazione client</span><span class="sxs-lookup"><span data-stu-id="3a1e4-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="3a1e4-103">I profili dei certificati client Intune NDES/SCEP e PKCS/PFX sono generalmente usati insieme ad altri tipi di profili, come Wi-Fi, VPN e posta elettronica, per consentire agli utenti di eseguire l'autenticazione alle risorse aziendali.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="3a1e4-104">Quando tali tipi di profilo sono collegati a un profilo di certificato client, essi dipendono dalla riuscita della distribuzione di quel profilo.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="3a1e4-105">La configurazione iniziale dell'infrastruttura e la configurazione associata del profilo del certificato client richiedono spesso la risoluzione di problemi.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="3a1e4-106">Per una guida dettagliata sulla configurazione efficace del connettore NDES e indicazioni di risoluzione per isolare i problemi relativi alla distribuzione dei certificati, vedere:</span><span class="sxs-lookup"><span data-stu-id="3a1e4-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="3a1e4-107">Configurare l'infrastruttura per supportare SCEP con Intune</span><span class="sxs-lookup"><span data-stu-id="3a1e4-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="3a1e4-108">Panoramica per la risoluzione dei problemi relativi ai profili dei certificati SCEP con Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3a1e4-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="3a1e4-109">Usare i riferimenti agli script di PowerShell per verificare la configurazione.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="3a1e4-110">Per altre informazioni, vedere [Script di verifica del connettore di certificati Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="3a1e4-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="3a1e4-111">**Altri problemi comuni**</span><span class="sxs-lookup"><span data-stu-id="3a1e4-111">**Other common issues**</span></span>

<span data-ttu-id="3a1e4-112">**Quando si prova a installare il connettore di certificati Intune nel server del connettore NDES, viene visualizzato il messaggio "La password nella richiesta di certificato non può essere verificata. Potrebbe essere già stata usata. Ottenere una nuova password da inviare con la richiesta."**</span><span class="sxs-lookup"><span data-stu-id="3a1e4-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="3a1e4-113">Questo messaggio indica che è necessario eseguire l'installazione del connettore di certificati come amministratore.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="3a1e4-114">In alcuni ambienti, i server in cui è in esecuzione il certificato Intune devono usare un server proxy per connettersi a Intune, quindi il connettore di certificati deve usare un proxy.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="3a1e4-115">In alcuni casi, il connettore NDES ignora le impostazioni proxy configurate e può essere necessario configurare le impostazioni proxy durante l'esecuzione nel contesto di sicurezza di LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="3a1e4-116">La soluzione è quella di eseguire Internet Explorer come sistema e configurare un proxy in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="3a1e4-117">Dopo il riavvio del servizio connettore di Intune, il connettore NDES si connette a Intune.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="3a1e4-118">**I dispositivi degli utenti non riceveranno più certificati SCEP da NDES.**</span><span class="sxs-lookup"><span data-stu-id="3a1e4-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="3a1e4-119">È possibile che il certificato di autenticazione client rilasciato al server NDES e specificato durante l'installazione del connettore NDES sia scaduto o mancante.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="3a1e4-120">Per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="3a1e4-120">To resolve:</span></span> 
 
1. <span data-ttu-id="3a1e4-121">Disinstallare il connettore NDES.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="3a1e4-122">Usare questi dettagli per richiedere un nuovo certificato di autenticazione client o un certificato di autenticazione server:</span><span class="sxs-lookup"><span data-stu-id="3a1e4-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="3a1e4-123">Nome del soggetto: CN = FQDN esterno</span><span class="sxs-lookup"><span data-stu-id="3a1e4-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="3a1e4-124">Nome alternativo del soggetto (entrambi obbligatori): DNS = FQDN esterno, DNS = FQDN interno</span><span class="sxs-lookup"><span data-stu-id="3a1e4-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="3a1e4-125">Reinstallare il connettore NDES con il nuovo certificato.</span><span class="sxs-lookup"><span data-stu-id="3a1e4-125">Reinstall the NDES connector with the new certificate.</span></span>