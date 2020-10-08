---
title: Distribuzione delle app Win32 con Intune
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
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366526"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="bc079-102">Distribuzione delle app Win32 con Intune</span><span class="sxs-lookup"><span data-stu-id="bc079-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="bc079-103">Microsoft Intune consente di distribuire le applicazioni Win32, inclusi MSI e i file .EXE, sui dispositivi Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bc079-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="bc079-104">Il meccanismo di distribuzione usato richiede che l’estensione Intune Management Extension (IME) sia installata sul dispositivo di destinazione.</span><span class="sxs-lookup"><span data-stu-id="bc079-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="bc079-105">L’estensione IME è installata automaticamente dopo che lo script di PowerShell o la distribuzione dell’applicazione Win32 sono associati a un utente/dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc079-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="bc079-106">La distribuzione delle app Win32 prevede anche una serie di prerequisiti da soddisfare, tra cui:</span><span class="sxs-lookup"><span data-stu-id="bc079-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="bc079-107">Piattaforme supportate: Windows 10 versione 1607 o successiva (versioni Enterprise, Pro ed Education)</span><span class="sxs-lookup"><span data-stu-id="bc079-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="bc079-108">Architettura supportata: x86 e x64.</span><span class="sxs-lookup"><span data-stu-id="bc079-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="bc079-109">Gestione dispositivi: AAD connesso e registrato automaticamente (inclusi i domini ibridi aggiunti e i criteri di gruppo registrati automaticamente).</span><span class="sxs-lookup"><span data-stu-id="bc079-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="bc079-110">Formato pacchetto dell’applicazione: file .**intunewin** preparato dallo strumento [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="bc079-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="bc079-111">Limitazioni:</span><span class="sxs-lookup"><span data-stu-id="bc079-111">Limitations:</span></span>
    - <span data-ttu-id="bc079-112">Dimensione massima: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="bc079-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="bc079-113">Architettura supportata: ARM.</span><span class="sxs-lookup"><span data-stu-id="bc079-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="bc079-114">Consultare il documento "[Aggiungere, assegnare e monitorare app Win32 in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" per le informazioni su questi passaggi.</span><span class="sxs-lookup"><span data-stu-id="bc079-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="bc079-115">I dettagli per risoluzione dei problemi di distribuzione su Windows, incluse le app Win32, sono disponibili nei seguenti documenti</span><span class="sxs-lookup"><span data-stu-id="bc079-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="bc079-116">Risoluzione dei problemi di installazione delle app</span><span class="sxs-lookup"><span data-stu-id="bc079-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="bc079-117">Risoluzione dei problemi delle app Win32</span><span class="sxs-lookup"><span data-stu-id="bc079-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)