---
title: Gestione dell'elenco indirizzi globale e della rubrica offline dell'organizzazione
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812695"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="b2d79-102">Gestione dell'elenco indirizzi globale e della rubrica offline dell'organizzazione</span><span class="sxs-lookup"><span data-stu-id="b2d79-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="b2d79-103">Un elenco indirizzi globale è un elenco di oggetti abilitati per la posta elettronica, ossia qualunque tipo di destinatario che può ricevere un messaggio di posta elettronica, all'interno dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b2d79-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="b2d79-104">In ogni organizzazione viene creato automaticamente un elenco indirizzi globale.</span><span class="sxs-lookup"><span data-stu-id="b2d79-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="b2d79-105">È possibile creare altri elenchi indirizzi globali per separare gli utenti in base all'organizzazione o al luogo, ma ogni utente può visualizzare e usare un solo elenco indirizzi globale per volta.</span><span class="sxs-lookup"><span data-stu-id="b2d79-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="b2d79-106">Alcuni client di posta elettronica, come Outlook per Windows, scaricano l'elenco indirizzi globale per l'uso offline.</span><span class="sxs-lookup"><span data-stu-id="b2d79-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="b2d79-107">Questo elenco è denominato rubrica offline.</span><span class="sxs-lookup"><span data-stu-id="b2d79-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="b2d79-108">In Exchange Online, una rubrica offline viene aggiornata ogni 8 ore, quindi i client devono scaricarla per aggiornare la copia offline locale.</span><span class="sxs-lookup"><span data-stu-id="b2d79-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="b2d79-109">Qualsiasi modifica ai destinatari deve essere visibile nell'elenco indirizzi globale prima di passare alla rubrica offline.</span><span class="sxs-lookup"><span data-stu-id="b2d79-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="b2d79-110">Di seguito sono riportate alcune procedure comuni per l'elenco indirizzi globale e la rubrica offline:</span><span class="sxs-lookup"><span data-stu-id="b2d79-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="b2d79-111">Per vari motivi, può essere preferibile che alcuni oggetti siano nascosti dall'elenco indirizzi globale.</span><span class="sxs-lookup"><span data-stu-id="b2d79-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="b2d79-112">Per ulteriori informazioni, vedere [Nascondere i destinatari dagli elenchi di indirizzi](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="b2d79-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="b2d79-113">Se è necessario assegnare visualizzazioni personalizzate dell'elenco indirizzi globale dell'organizzazione a specifici gruppi di utenti, vedere [Criteri della rubrica in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="b2d79-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="b2d79-114">[Creare un elenco indirizzi globale in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) e vedere [Elenchi di indirizzi in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) per informazioni sull'uso delle autorizzazioni dell'elenco indirizzo globale.</span><span class="sxs-lookup"><span data-stu-id="b2d79-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="b2d79-115">Tenere presente che, se si crea un nuovo elenco indirizzi globale, può essere utile creare anche una nuova rubrica offline.</span><span class="sxs-lookup"><span data-stu-id="b2d79-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="b2d79-116">Vedere [Procedure relative alle rubriche offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="b2d79-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
