---
title: Elenchi di grandi dimensioni di SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720137"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="64c9c-102">Utilizzo di elenchi e raccolte di grandi dimensioni in SharePoint</span><span class="sxs-lookup"><span data-stu-id="64c9c-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="64c9c-103">Gli elenchi e le raccolte di SharePoint possono contenere fino a 30 milioni elementi, ma quando dispongono di più di 5.000 elementi, è possibile che venga visualizzato un errore di soglia per la visualizzazione elenco quando si tenta di utilizzarli.</span><span class="sxs-lookup"><span data-stu-id="64c9c-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="64c9c-104">Questa soglia è pensata per garantire le prestazioni del servizio</span><span class="sxs-lookup"><span data-stu-id="64c9c-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="64c9c-105">e non può essere modificata.</span><span class="sxs-lookup"><span data-stu-id="64c9c-105">It can't be changed.</span></span> <span data-ttu-id="64c9c-106">Per evitare di colpire questa soglia:</span><span class="sxs-lookup"><span data-stu-id="64c9c-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="64c9c-107">**USA moderna**</span><span class="sxs-lookup"><span data-stu-id="64c9c-107">**Use modern**</span></span>

<span data-ttu-id="64c9c-108">Le visualizzazioni che mostrano molti elementi funzionano meglio nell'esperienza moderna.</span><span class="sxs-lookup"><span data-stu-id="64c9c-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="64c9c-109">[Utilizzare l'esperienza moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) per evitare errori che potrebbero essere visualizzati nell'esperienza classica.</span><span class="sxs-lookup"><span data-stu-id="64c9c-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="64c9c-110">**Aggiungere indici**</span><span class="sxs-lookup"><span data-stu-id="64c9c-110">**Add indexes**</span></span>

<span data-ttu-id="64c9c-111">Quando si filtra o si ordina in base a una colonna che non dispone di un indice, è possibile che venga visualizzato un messaggio di errore.</span><span class="sxs-lookup"><span data-stu-id="64c9c-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="64c9c-112">[Aggiungere un indice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente dalle **impostazioni dell'elenco** nel menu impostazioni, quindi **colonne indicizzate**.</span><span class="sxs-lookup"><span data-stu-id="64c9c-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="64c9c-113">**Modificare la visualizzazione elenco**</span><span class="sxs-lookup"><span data-stu-id="64c9c-113">**Edit the list view**</span></span>

<span data-ttu-id="64c9c-114">Se si verifica un errore durante l'utilizzo di un elenco di grandi dimensioni, [modificare la visualizzazione elenco](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="64c9c-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="64c9c-115">Le quattro modifiche seguenti elimineranno gli errori di soglia della visualizzazione elenco.</span><span class="sxs-lookup"><span data-stu-id="64c9c-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="64c9c-116">Apportare tutte e quattro le modifiche per rimuovere tutti gli errori.</span><span class="sxs-lookup"><span data-stu-id="64c9c-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="64c9c-117">Se si verificano ancora errori, controllare la [gestione di elenchi e raccolte di grandi dimensioni](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="64c9c-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="64c9c-118">Selezionare **None** dal **primo ordinamento in base alla colonna** e **quindi ordinare in base alla colonna**.</span><span class="sxs-lookup"><span data-stu-id="64c9c-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="64c9c-119">Selezionare **None** dal **primo gruppo in base alla colonna** e **quindi raggruppare in base alla colonna**.</span><span class="sxs-lookup"><span data-stu-id="64c9c-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="64c9c-120">Selezionare **Nessuna** per tutte le colonne nella sezione **totali** .</span><span class="sxs-lookup"><span data-stu-id="64c9c-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="64c9c-121">Deselezionare tutte le colonne, tranne una per la visualizzazione, dalla sezione **Columns** .</span><span class="sxs-lookup"><span data-stu-id="64c9c-121">Deselect all but one column for display from the **Columns** section.</span></span>

