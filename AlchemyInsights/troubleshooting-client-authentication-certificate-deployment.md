---
title: Risoluzione dei problemi relativi alla distribuzione del certificato di autenticazione client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658990"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Risoluzione dei problemi relativi alla distribuzione del certificato di autenticazione client

I profili dei certificati client Intune NDES/SCEP e PKCS/PFX sono generalmente usati insieme ad altri tipi di profili, come Wi-Fi, VPN e posta elettronica, per consentire agli utenti di eseguire l'autenticazione alle risorse aziendali. Quando tali tipi di profilo sono collegati a un profilo di certificato client, essi dipendono dalla riuscita della distribuzione di quel profilo.

La configurazione iniziale dell'infrastruttura e la configurazione associata del profilo del certificato client richiedono spesso la risoluzione di problemi. Per una guida dettagliata sulla configurazione efficace del connettore NDES e indicazioni di risoluzione per isolare i problemi relativi alla distribuzione dei certificati, vedere: 

- [Configurare l'infrastruttura per supportare SCEP con Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Panoramica per la risoluzione dei problemi relativi ai profili dei certificati SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Usare i riferimenti agli script di PowerShell per verificare la configurazione. Per altre informazioni, vedere [Script di verifica del connettore di certificati Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Altri problemi comuni**

**Quando si prova a installare il connettore di certificati Intune nel server del connettore NDES, viene visualizzato il messaggio "La password nella richiesta di certificato non può essere verificata. Potrebbe essere già stata usata. Ottenere una nuova password da inviare con la richiesta."**  

Questo messaggio indica che è necessario eseguire l'installazione del connettore di certificati come amministratore.

In alcuni ambienti, i server in cui è in esecuzione il certificato Intune devono usare un server proxy per connettersi a Intune, quindi il connettore di certificati deve usare un proxy. In alcuni casi, il connettore NDES ignora le impostazioni proxy configurate e può essere necessario configurare le impostazioni proxy durante l'esecuzione nel contesto di sicurezza di LocalSystem. 
 
La soluzione è quella di eseguire Internet Explorer come sistema e configurare un proxy in Internet Explorer. Dopo il riavvio del servizio connettore di Intune, il connettore NDES si connette a Intune.

**I dispositivi degli utenti non riceveranno più certificati SCEP da NDES.**

È possibile che il certificato di autenticazione client rilasciato al server NDES e specificato durante l'installazione del connettore NDES sia scaduto o mancante. Per risolvere il problema: 
 
1. Disinstallare il connettore NDES.  
2. Usare questi dettagli per richiedere un nuovo certificato di autenticazione client o un certificato di autenticazione server: 
 
    - Nome del soggetto: CN = FQDN esterno  
    - Nome alternativo del soggetto (entrambi obbligatori): DNS = FQDN esterno, DNS = FQDN interno 
 
3. Reinstallare il connettore NDES con il nuovo certificato.