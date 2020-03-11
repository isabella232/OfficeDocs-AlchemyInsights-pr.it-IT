---
title: Utilizzare l'opzione di sblocco dell'impronta digitale in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588320"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utilizzare l'opzione di sblocco dell'impronta digitale in Windows 10

**Abilitazione di Windows Hello Fingerprint**

Per sbloccare Windows 10 con l'impronta digitale, è necessario configurare Windows Hello Fingerprint aggiungendo (lasciando Windows Learn to recognize) almeno un dito. 

1. Andare a **impostazioni > account > opzioni di accesso** (o fare clic [qui](ms-settings:signinoptions?activationSource=GetHelp)). Vengono elencate le opzioni di accesso disponibili. Ad esempio:

    ![Opzioni di accesso.](media/sign-in-options.png)

2. Fare clic o toccare **Windows Hello Fingerprint**, quindi fare clic su **Configura**. Nella finestra del programma di installazione di Windows Hello fare clic su **inizia**. Il sensore di impronte digitali si attiverà e ti verrà richiesto di posizionare il dito sul sensore:

   ![Sensore di impronte digitali.](media/fingerprint-sensor.png)

3. Segui le istruzioni, in cui viene chiesto di eseguire la scansione ripetuta del dito. Al termine, si avrà la possibilità di aggiungere altre dita che si desidera utilizzare per l'accesso. La volta successiva che si accede a Windows 10, si avrà la possibilità di utilizzare l'impronta digitale per farlo.

**Windows Hello Fingerprint non disponibile come opzione di accesso**

Se Windows Hello Fingerprint non è visualizzato come opzione nelle **Opzioni di accesso**, significa che Windows non è a conoscenza di un lettore/scanner di impronte digitali collegato al PC o che un criterio di sistema ne impedisce l'utilizzo (se ad esempio il PC è gestito dal proprio ambiente di lavoro). Per risolvere i problemi: 

1. Selezionare il pulsante **Start** nella barra delle applicazioni e cercare **Gestione dispositivi**.

2. Fare clic o toccare per aprire **Gestione dispositivi**.

3. In gestione dispositivi espandere i dispositivi biometrici facendo clic sul relativo Chevron.

   ![Dispositivi biometrici.](media/biometric-devices.png)

4. Lo scanner di impronte digitali dovrebbe essere elencato come dispositivo biometrico, ad esempio lo scanner Synaptics WBDI:

   ![Dispositivi biometrici.](media/biometric-devices-expanded.png)

5. Se lo scanner di impronte digitali non è visualizzato e lo scanner è integrato nel PC, passare al sito Web del produttore del PC. Nella sezione supporto tecnico per il modello di PC, cercare un driver di Windows 10 per uno scanner che è possibile installare.

6. Se lo scanner è separato dal PC (collegato tramite USB), passare al sito Web del produttore dello scanner per individuare e installare il software del driver di dispositivo di Windows 10 per il modello dello scanner di cui si dispone.
