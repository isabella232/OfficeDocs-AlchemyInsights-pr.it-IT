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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2d291-102">Utilizzare l'opzione di sblocco dell'impronta digitale in Windows 10</span><span class="sxs-lookup"><span data-stu-id="2d291-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2d291-103">**Abilitazione di Windows Hello Fingerprint**</span><span class="sxs-lookup"><span data-stu-id="2d291-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2d291-104">Per sbloccare Windows 10 con l'impronta digitale, è necessario configurare Windows Hello Fingerprint aggiungendo (lasciando Windows Learn to recognize) almeno un dito.</span><span class="sxs-lookup"><span data-stu-id="2d291-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2d291-105">Andare a **impostazioni > account > opzioni di accesso** (o fare clic [qui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="2d291-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2d291-106">Vengono elencate le opzioni di accesso disponibili.</span><span class="sxs-lookup"><span data-stu-id="2d291-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2d291-107">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="2d291-107">For example:</span></span>

    ![Opzioni di accesso.](media/sign-in-options.png)

2. <span data-ttu-id="2d291-109">Fare clic o toccare **Windows Hello Fingerprint**, quindi fare clic su **Configura**.</span><span class="sxs-lookup"><span data-stu-id="2d291-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2d291-110">Nella finestra del programma di installazione di Windows Hello fare clic su **inizia**.</span><span class="sxs-lookup"><span data-stu-id="2d291-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2d291-111">Il sensore di impronte digitali si attiverà e ti verrà richiesto di posizionare il dito sul sensore:</span><span class="sxs-lookup"><span data-stu-id="2d291-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensore di impronte digitali.](media/fingerprint-sensor.png)

3. <span data-ttu-id="2d291-113">Segui le istruzioni, in cui viene chiesto di eseguire la scansione ripetuta del dito.</span><span class="sxs-lookup"><span data-stu-id="2d291-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2d291-114">Al termine, si avrà la possibilità di aggiungere altre dita che si desidera utilizzare per l'accesso.</span><span class="sxs-lookup"><span data-stu-id="2d291-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2d291-115">La volta successiva che si accede a Windows 10, si avrà la possibilità di utilizzare l'impronta digitale per farlo.</span><span class="sxs-lookup"><span data-stu-id="2d291-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2d291-116">**Windows Hello Fingerprint non disponibile come opzione di accesso**</span><span class="sxs-lookup"><span data-stu-id="2d291-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2d291-117">Se Windows Hello Fingerprint non è visualizzato come opzione nelle **Opzioni di accesso**, significa che Windows non è a conoscenza di un lettore/scanner di impronte digitali collegato al PC o che un criterio di sistema ne impedisce l'utilizzo (se ad esempio il PC è gestito dal proprio ambiente di lavoro).</span><span class="sxs-lookup"><span data-stu-id="2d291-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2d291-118">Per risolvere i problemi:</span><span class="sxs-lookup"><span data-stu-id="2d291-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2d291-119">Selezionare il pulsante **Start** nella barra delle applicazioni e cercare **Gestione dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="2d291-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2d291-120">Fare clic o toccare per aprire **Gestione dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="2d291-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2d291-121">In gestione dispositivi espandere i dispositivi biometrici facendo clic sul relativo Chevron.</span><span class="sxs-lookup"><span data-stu-id="2d291-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivi biometrici.](media/biometric-devices.png)

4. <span data-ttu-id="2d291-123">Lo scanner di impronte digitali dovrebbe essere elencato come dispositivo biometrico, ad esempio lo scanner Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="2d291-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivi biometrici.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2d291-125">Se lo scanner di impronte digitali non è visualizzato e lo scanner è integrato nel PC, passare al sito Web del produttore del PC.</span><span class="sxs-lookup"><span data-stu-id="2d291-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2d291-126">Nella sezione supporto tecnico per il modello di PC, cercare un driver di Windows 10 per uno scanner che è possibile installare.</span><span class="sxs-lookup"><span data-stu-id="2d291-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2d291-127">Se lo scanner è separato dal PC (collegato tramite USB), passare al sito Web del produttore dello scanner per individuare e installare il software del driver di dispositivo di Windows 10 per il modello dello scanner di cui si dispone.</span><span class="sxs-lookup"><span data-stu-id="2d291-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
