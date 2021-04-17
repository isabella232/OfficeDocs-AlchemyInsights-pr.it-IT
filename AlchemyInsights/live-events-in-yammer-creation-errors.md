---
title: Errori di creazione di eventi live in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825519"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="76426-102">Errori di creazione di eventi live in Yammer</span><span class="sxs-lookup"><span data-stu-id="76426-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="76426-103">**Creazione di eventi live in Yammer**</span><span class="sxs-lookup"><span data-stu-id="76426-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="76426-104">Yammer mostra sempre l'opzione per creare un evento live.</span><span class="sxs-lookup"><span data-stu-id="76426-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="76426-105">In alcuni casi, è possibile che un utente non soddisfi i prerequisiti per la creazione di un evento live e che venga visualizzato un messaggio di errore quando tenta di crearlo.</span><span class="sxs-lookup"><span data-stu-id="76426-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="76426-106">Di seguito sono indicate le cause più comuni di questo problema e sono illustrati alcuni modi per risolverlo per gli utenti finali.</span><span class="sxs-lookup"><span data-stu-id="76426-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="76426-107">**Chi può creare eventi live**</span><span class="sxs-lookup"><span data-stu-id="76426-107">**Who can create live events**</span></span>
- <span data-ttu-id="76426-108">Una licenza di Office 365 Enterprise E1, E3 o E5 o una licenza di Office 365 A3 o A5.</span><span class="sxs-lookup"><span data-stu-id="76426-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="76426-109">Autorizzazioni per la creazione di eventi live nell'interfaccia di amministrazione di Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="76426-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="76426-110">Autorizzazioni per la creazione di eventi live in Microsoft Stream (per gli eventi prodotti con un'app o un dispositivo di trasmissione esterno).</span><span class="sxs-lookup"><span data-stu-id="76426-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="76426-111">Appartenenza completa a un team dell'organizzazione (non si può essere guest o di un'altra organizzazione).</span><span class="sxs-lookup"><span data-stu-id="76426-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="76426-112">Pianificazione di riunioni private, condivisione dello schermo e condivisione di video IP attivate nei criteri per le riunioni del team.</span><span class="sxs-lookup"><span data-stu-id="76426-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="76426-113">**Criteri di creazione di eventi live**</span><span class="sxs-lookup"><span data-stu-id="76426-113">**Live event creation policies**</span></span>

<span data-ttu-id="76426-114">Yammer segue i criteri per gli eventi live impostati nel tenant di Office 365 per Stream.</span><span class="sxs-lookup"><span data-stu-id="76426-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="76426-115">Per impostazione predefinita, tutti gli utenti dell'organizzazione possono creare un evento live.</span><span class="sxs-lookup"><span data-stu-id="76426-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="76426-116">Gli amministratori potrebbero [apportare modifiche a questa impostazione che potrebbero impedire agli utenti di creare un evento live](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="76426-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="76426-117">È importante verificare che gli utenti dispongano delle autorizzazioni per creare eventi live se ricevono un errore relativo ai criteri.</span><span class="sxs-lookup"><span data-stu-id="76426-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
