---
title: Usare l'opzione di sblocco delle impronte digitali in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971939"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Usare l'opzione di sblocco delle impronte digitali in Windows 10

**Abilita impronta Windows Hello digitale**

Per sbloccare Windows 10 tramite l'impronta digitale, devi configurare l'impronta digitale Windows Hello aggiungendo (consentendo Windows imparare a riconoscere) almeno un dito. 

1. Vai a **Impostazioni > account > opzioni di accesso** (o fai clic [qui](ms-settings:signinoptions?activationSource=GetHelp)). Verranno elencate le opzioni di accesso disponibili. Ad esempio:

    ![Opzioni di accesso.](media/sign-in-options.png)

2. Tocca o fai **clic Windows Hello'impronta digitale** e quindi fai clic **su Configura.** Nella finestra Windows Hello di installazione fare clic su **Introduzione.** Il sensore di impronta digitale si attiverà e ti verrà chiesto di posizionare il dito sul sensore:

   ![Sensore di impronta digitale.](media/fingerprint-sensor.png)

3. Segui le istruzioni, che ti chiederanno di eseguire ripetutamente la scansione del dito. Al termine, avrai la possibilità di aggiungere altre dita che potresti voler usare per l'accesso. Al successivo accesso a Windows 10, sarà possibile usare l'impronta digitale per farlo.

**Windows Hello Impronta digitale non disponibile come opzione di accesso**

Se Windows Hello Fingerprint non è visualizzata come opzione **in** Opzioni di accesso, significa che Windows non è a conoscenza di alcun lettore/scanner di impronte digitali collegato al PC o che un criterio di sistema ne impedisce l'uso (se ad esempio il PC è gestito dall'area di lavoro). Per risolvere i problemi: 

1. Seleziona il **pulsante Start** nella barra delle applicazioni e cerca **Gestione dispositivi.**

2. Toccare o fare clic per aprire **Gestione dispositivi.**

3. In Gestione dispositivi espandi Dispositivi biometrici facendo clic sul relativo chevron.

   ![Dispositivi biometrici.](media/biometric-devices.png)

4. Lo scanner di impronte digitali deve essere elencato come dispositivo biometrico, ad esempio lo scanner Synaptics WBDI:

   ![Dispositivi biometrici.](media/biometric-devices-expanded.png)

5. Se lo scanner di impronte digitali non viene visualizzato e lo scanner è integrato nel PC, accedere al sito Web del produttore del PC. Nella sezione supporto tecnico per il modello di PC, cercare un driver Windows 10 driver per uno scanner che è possibile installare.

6. Se lo scanner è separato dal PC (collegato tramite USB), accedere al sito Web del produttore dello scanner per trovare e installare il software del driver di dispositivo Windows 10 per il modello di scanner in uso.
