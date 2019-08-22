---
title: File aperto di sola lettura
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 5c28d5f1c6951971aab329060e24b8458e848dd7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525675"
---
# <a name="file-open-read-only"></a><span data-ttu-id="abaad-102">File aperto di sola lettura</span><span class="sxs-lookup"><span data-stu-id="abaad-102">File open read-only</span></span>

<span data-ttu-id="abaad-103">Quando si aprono file, è possibile che si aprano come di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="abaad-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="abaad-104">In alcuni casi, si tratta di una sicurezza aggiuntiva, ad esempio quando si aprono file da Internet e altre volte, può essere dovuto a un'impostazione che può essere modificata.</span><span class="sxs-lookup"><span data-stu-id="abaad-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="abaad-105">Di seguito sono riportati alcuni scenari in cui un file viene aperto in sola lettura e alcuni passaggi che è possibile eseguire per modificarlo.</span><span class="sxs-lookup"><span data-stu-id="abaad-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="abaad-106">**Il mio antivirus sta facendo in modo che apra la sola lettura**</span><span class="sxs-lookup"><span data-stu-id="abaad-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="abaad-107">Alcuni programmi antivirus possono proteggersi da file potenzialmente non sicuri aprendoli di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="abaad-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="abaad-108">Potrebbe essere necessario verificare con il provider di servizi antivirus per informazioni su come modificare queste impostazioni.</span><span class="sxs-lookup"><span data-stu-id="abaad-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="abaad-109">BitDefender, ad esempio, ha contenuto per l'aggiunta di esclusioni di applicazioni qui: [come aggiungere esclusioni di applicazioni o processi nel centro di controllo di BitDefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="abaad-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="abaad-110">**Le proprietà del file sono impostate come di sola lettura?**</span><span class="sxs-lookup"><span data-stu-id="abaad-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="abaad-111">È possibile controllare le proprietà del file facendo clic con il pulsante destro del mouse sul file e scegliendo Proprietà.</span><span class="sxs-lookup"><span data-stu-id="abaad-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="abaad-112">Se l'attributo di sola lettura è selezionato, è possibile deselezionarlo e fare clic su OK.</span><span class="sxs-lookup"><span data-stu-id="abaad-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="abaad-113">**Il contenuto è in visualizzazione protetta**</span><span class="sxs-lookup"><span data-stu-id="abaad-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="abaad-114">I file provenienti da Internet e da altri percorsi potenzialmente non sicuri possono contenere virus, worm o altri tipi di malware che possono danneggiare il computer.</span><span class="sxs-lookup"><span data-stu-id="abaad-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="abaad-115">Si tratta in genere anche degli allegati di posta elettronica o dei file scaricati.</span><span class="sxs-lookup"><span data-stu-id="abaad-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="abaad-116">Per proteggere il computer, i file provenienti da questi percorsi potenzialmente non sicuri vengono aperti in visualizzazione protetta.</span><span class="sxs-lookup"><span data-stu-id="abaad-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="abaad-117">Se si utilizza la visualizzazione protetta, è possibile leggere un file e visualizzarne il contenuto riducendo i rischi.</span><span class="sxs-lookup"><span data-stu-id="abaad-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="abaad-118">Per ulteriori informazioni sulla visualizzazione protetta e su come modificare le impostazioni, vedere questo articolo: [che cos'è protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="abaad-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="abaad-119">**OneDrive è completo?**</span><span class="sxs-lookup"><span data-stu-id="abaad-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="abaad-120">Se il file è archiviato su OneDrive e lo spazio di archiviazione di OneDrive è pieno, non sarà possibile salvare il documento finché non si è sotto lo spazio assegnato.</span><span class="sxs-lookup"><span data-stu-id="abaad-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="abaad-121">È possibile controllare lo spazio disponibile su OneDrive facendo clic sull'icona di OneDrive nel centro notifiche e scegliendo Gestisci archiviazione oppure è possibile [http://onedrive.live.com](http://onedrive.live.com)accedere a, accedere e annotare la quantità di spazio utilizzato in basso a sinistra dello schermo.</span><span class="sxs-lookup"><span data-stu-id="abaad-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="abaad-122">**Office è attivato?**</span><span class="sxs-lookup"><span data-stu-id="abaad-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="abaad-123">Se Office non è attivato o se l'abbonamento è scaduto, è possibile che si trovi in modalità di sola lettura con funzionalità ridotte.</span><span class="sxs-lookup"><span data-stu-id="abaad-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="abaad-124">Per informazioni su come attivare Office, vedere: [errori di attivazione e di prodotto senza licenza in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="abaad-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="abaad-125">**Se tutto il resto ha esito negativo...**</span><span class="sxs-lookup"><span data-stu-id="abaad-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="abaad-126">Provare a riavviare il computer</span><span class="sxs-lookup"><span data-stu-id="abaad-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="abaad-127">Installare gli aggiornamenti di Office</span><span class="sxs-lookup"><span data-stu-id="abaad-127">Install Office updates</span></span>
    
- <span data-ttu-id="abaad-128">Eseguire un ripristino online di Office</span><span class="sxs-lookup"><span data-stu-id="abaad-128">Perform an Online repair of Office</span></span>
    

