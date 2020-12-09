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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599469"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="3e002-102">Accedere automaticamente a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3e002-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="3e002-103">Microsoft Edge utilizza l'account predefinito del sistema operativo per accedere automaticamente a un utente in base al modo in cui viene configurato il dispositivo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="3e002-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="3e002-104">Di seguito sono descritti gli scenari di ogni tipo di configurazione del dispositivo e del relativo processo di accesso dell'utente dipendente:</span><span class="sxs-lookup"><span data-stu-id="3e002-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="3e002-105">**Il dispositivo è ibrido/AAD-J**: questa opzione è disponibile in Windows 10, finestre di livello basso e versioni del server corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="3e002-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3e002-106">Gli utenti vengono automaticamente firmati con gli account di Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="3e002-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="3e002-107">**Il dispositivo è associato a un dominio**: questa opzione è disponibile in Windows 10, finestre di livello basso e versioni del server corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="3e002-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3e002-108">Per impostazione predefinita, gli utenti con account di dominio non sono firmati automaticamente. per abilitare l'accesso automatico per gli stessi, utilizzare il criterio **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="3e002-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="3e002-109">Per abilitare l'accesso automatico per gli utenti con account Azure AD, prendere in considerazione l'aggiunta ibrida dei propri dispositivi.</span><span class="sxs-lookup"><span data-stu-id="3e002-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="3e002-110">**L'account predefinito del sistema operativo è un account Microsoft**: questa opzione è disponibile in Windows 10 RS3 (versione 1709, Build 10.0.16299) e versioni successive.</span><span class="sxs-lookup"><span data-stu-id="3e002-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="3e002-111">Lo scenario è improbabile che si verifichi nei dispositivi Enterprise.</span><span class="sxs-lookup"><span data-stu-id="3e002-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="3e002-112">Tuttavia, se l'account predefinito del sistema operativo è un account Microsoft, Microsoft Edge accederà automaticamente all'utente con l'account Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3e002-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
