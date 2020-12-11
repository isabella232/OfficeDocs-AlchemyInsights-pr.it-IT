---
title: Utilizzo di Microsoft Intune per gestire l'accesso Web in Microsoft Edge per iOS e Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617281"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="2c36a-102">Utilizzo di Microsoft Intune per gestire l'accesso Web in Microsoft Edge per iOS e Android</span><span class="sxs-lookup"><span data-stu-id="2c36a-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="2c36a-103">Microsoft Edge per iOS e Android consente a un utente di esplorare il Web da più profili completamente separati.</span><span class="sxs-lookup"><span data-stu-id="2c36a-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="2c36a-104">Le più vaste funzionalità di protezione per i dati di Microsoft 365 diventano disponibili quando si sottoscrive la famiglia di prodotti Enterprise Mobility + Security, che include le funzionalità di Microsoft Intune e Azure Active Directory Premium, ad esempio l'accesso condizionale.</span><span class="sxs-lookup"><span data-stu-id="2c36a-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="2c36a-105">È necessario distribuire un criterio di accesso condizionale che (1) consente agli utenti di connettersi da dispositivi mobili a Microsoft Edge per iOS e Android e che (2) implementi un criterio di protezione delle app di Microsoft Intune che fornisce un'esperienza di esplorazione protetta.</span><span class="sxs-lookup"><span data-stu-id="2c36a-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="2c36a-106">Per comprendere come è possibile utilizzare i criteri e l'accesso condizionale, vedere:</span><span class="sxs-lookup"><span data-stu-id="2c36a-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="2c36a-107">Applicare i criteri di accesso condizionale di Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2c36a-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="2c36a-108">Creare criteri di protezione delle app di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2c36a-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="2c36a-109">Utilizzo del servizio Single Sign-on per le app Web di Azure Active Directory connesse nei browser protetti da criteri</span><span class="sxs-lookup"><span data-stu-id="2c36a-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="2c36a-110">Utilizzare la configurazione delle app per gestire l'esperienza di esplorazione</span><span class="sxs-lookup"><span data-stu-id="2c36a-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="2c36a-111">Consenti l'utilizzo di solo account scolastici e di lavoro</span><span class="sxs-lookup"><span data-stu-id="2c36a-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="2c36a-112">Distribuire i criteri generali di configurazione delle app</span><span class="sxs-lookup"><span data-stu-id="2c36a-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="2c36a-113">Distribuire i criteri di configurazione delle app per la protezione dei dati</span><span class="sxs-lookup"><span data-stu-id="2c36a-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="2c36a-114">Utilizzo di Microsoft Endpoint Manager per la distribuzione di criteri di configurazione delle app</span><span class="sxs-lookup"><span data-stu-id="2c36a-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="2c36a-115">Per informazioni su come accedere ai log delle app gestite, vedere [usare Microsoft Edge per iOS e Android per accedere ai log delle app gestite](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="2c36a-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
