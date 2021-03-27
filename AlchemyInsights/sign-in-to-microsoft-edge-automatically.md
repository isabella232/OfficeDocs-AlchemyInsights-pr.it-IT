---
title: Accedere automaticamente a Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398733"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="22213-102">Accedere automaticamente a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="22213-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="22213-103">Microsoft Edge usa l'account predefinito del sistema operativo per accedere automaticamente a un utente in base alla configurazione del dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="22213-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="22213-104">Di seguito sono descritti gli scenari di ogni tipo di configurazione del dispositivo e del relativo processo di accesso utente dipendente:</span><span class="sxs-lookup"><span data-stu-id="22213-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="22213-105">**Il dispositivo è ibrido/AAD-J:** questa opzione è disponibile in Windows 10, Windows di livello inferiore e versioni server corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="22213-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="22213-106">Gli utenti hanno eseguito automaticamente l'accesso con i propri account Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="22213-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="22213-107">**Il dispositivo è aggiunto al** dominio: questa opzione è disponibile in Windows 10, windows di livello inferiore e versioni server corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="22213-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="22213-108">Per impostazione predefinita, gli utenti con account di dominio non vengono connessi automaticamente. per abilitare l'accesso automatico, utilizzare il **criterio ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="22213-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="22213-109">Per abilitare l'accesso automatico per gli utenti con account Azure AD, prendi in considerazione l'aggiunta ibrida dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="22213-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="22213-110">L'account predefinito del sistema operativo è un **account Microsoft:** questa opzione è disponibile in Windows 10 RS3 (versione 1709, build 10.0.16299) e versioni successive.</span><span class="sxs-lookup"><span data-stu-id="22213-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="22213-111">È improbabile che lo scenario si verifichi nei dispositivi aziendali.</span><span class="sxs-lookup"><span data-stu-id="22213-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="22213-112">Tuttavia, se l'account predefinito del sistema operativo è un account Microsoft, Microsoft Edge accederà automaticamente all'utente con l'account Microsoft.</span><span class="sxs-lookup"><span data-stu-id="22213-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
