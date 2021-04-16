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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796681"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e9909-102">Usare l'opzione di sblocco delle impronte digitali in Windows 10</span><span class="sxs-lookup"><span data-stu-id="e9909-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e9909-103">**Abilitare l'impronta digitale di Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="e9909-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e9909-104">Per sbloccare Windows 10 usando l'impronta digitale, devi configurare l'impronta digitale di Windows Hello aggiungendo (consentendo a Windows di riconoscere) almeno un dito.</span><span class="sxs-lookup"><span data-stu-id="e9909-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e9909-105">Vai a **Impostazioni > account > opzioni di** accesso (o fai clic [qui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="e9909-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e9909-106">Verranno elencate le opzioni di accesso disponibili.</span><span class="sxs-lookup"><span data-stu-id="e9909-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e9909-107">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="e9909-107">For example:</span></span>

    ![Opzioni di accesso.](media/sign-in-options.png)

2. <span data-ttu-id="e9909-109">Tocca o fai clic **su Impronta digitale di Windows Hello,** quindi fai clic su **Configura.**</span><span class="sxs-lookup"><span data-stu-id="e9909-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e9909-110">Nella finestra di installazione di Windows Hello fai clic su **Introduzione.**</span><span class="sxs-lookup"><span data-stu-id="e9909-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e9909-111">Il sensore di impronta digitale si attiverà e ti verrà chiesto di posizionare il dito sul sensore:</span><span class="sxs-lookup"><span data-stu-id="e9909-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensore di impronta digitale.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e9909-113">Segui le istruzioni, che ti chiederanno di eseguire ripetutamente la scansione del dito.</span><span class="sxs-lookup"><span data-stu-id="e9909-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e9909-114">Al termine, avrai la possibilità di aggiungere altre dita che potresti voler usare per l'accesso.</span><span class="sxs-lookup"><span data-stu-id="e9909-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e9909-115">Al successivo accesso a Windows 10, potrai usare l'impronta digitale per farlo.</span><span class="sxs-lookup"><span data-stu-id="e9909-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e9909-116">**Impronta digitale di Windows Hello non disponibile come opzione di accesso**</span><span class="sxs-lookup"><span data-stu-id="e9909-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e9909-117">Se l'impronta digitale di Windows Hello non è visualizzata come opzione **in** Opzioni di accesso, significa che Windows non è a conoscenza di alcun lettore/scanner di impronte digitali collegato al PC o che un criterio di sistema ne impedisce l'uso (se ad esempio il PC è gestito dall'area di lavoro).</span><span class="sxs-lookup"><span data-stu-id="e9909-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e9909-118">Per risolvere i problemi:</span><span class="sxs-lookup"><span data-stu-id="e9909-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e9909-119">Seleziona il **pulsante Start** nella barra delle applicazioni e cerca **Gestione dispositivi.**</span><span class="sxs-lookup"><span data-stu-id="e9909-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e9909-120">Toccare o fare clic per aprire **Gestione dispositivi.**</span><span class="sxs-lookup"><span data-stu-id="e9909-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e9909-121">In Gestione dispositivi espandi Dispositivi biometrici facendo clic sul relativo chevron.</span><span class="sxs-lookup"><span data-stu-id="e9909-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivi biometrici.](media/biometric-devices.png)

4. <span data-ttu-id="e9909-123">Lo scanner di impronte digitali deve essere elencato come dispositivo biometrico, ad esempio lo scanner Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="e9909-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivi biometrici.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e9909-125">Se lo scanner di impronte digitali non viene visualizzato e lo scanner è integrato nel PC, accedere al sito Web del produttore del PC.</span><span class="sxs-lookup"><span data-stu-id="e9909-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e9909-126">Nella sezione supporto tecnico per il modello di PC cerca un driver di Windows 10 per uno scanner che puoi installare.</span><span class="sxs-lookup"><span data-stu-id="e9909-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e9909-127">Se lo scanner è separato dal PC (collegato tramite USB), accedere al sito Web del produttore dello scanner per trovare e installare il software del driver di dispositivo Windows 10 per il modello di scanner in uso.</span><span class="sxs-lookup"><span data-stu-id="e9909-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
