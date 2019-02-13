---
title: Utilizzo di iOS VPP applicazioni regola Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917500"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="c22cf-102">Utilizzo di iOS VPP applicazioni</span><span class="sxs-lookup"><span data-stu-id="c22cf-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="c22cf-103">Informazioni su [come gestire le app di iOS acquistato tramite un programma volume di acquisto con Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) informazioni sulle caratteristiche, vincoli e operazioni affinché utilizzare del programma di acquisto Volume Apple e il relativo supporto Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c22cf-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="c22cf-104">**Problemi comuni:** "Un'app di iOS VPP sono stati assegnati agli utenti, ma l'installazione non riuscita"</span><span class="sxs-lookup"><span data-stu-id="c22cf-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="c22cf-p101">Ciò può verificarsi se viene utilizzato un singolo token VPP tra più provider di gestione di dispositivi mobili. I token VPP Apple possono essere utilizzati solo con un provider. Se è stato utilizzato un token VPP con più provider, è necessario caricare nuovamente il token da Intune.</span><span class="sxs-lookup"><span data-stu-id="c22cf-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="c22cf-p102">L'installazione di esito negativo anche se il numero totale di installazioni supera il numero di licenze. Per visualizzare un report di utilizzo per le licenze, passare a **Intune Mobile App** \> pagina **licenze per l'applicazione** . Per informazioni su come liberare le licenze in uso, vedere [in questo articolo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="c22cf-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

