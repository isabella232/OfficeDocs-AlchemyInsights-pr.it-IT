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
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: be232b682b7bb3d24f59ad10501edbd796e6bcaf
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401757"
---
# <a name="file-open-read-only"></a><span data-ttu-id="a7b1e-102">File aperto di sola lettura</span><span class="sxs-lookup"><span data-stu-id="a7b1e-102">File open read-only</span></span>

<span data-ttu-id="a7b1e-103">Quando si aprono file, è possibile che si aprano come di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="a7b1e-104">In alcuni casi, si tratta di una sicurezza aggiuntiva, ad esempio quando si aprono file da Internet e altre volte, può essere dovuto a un'impostazione che può essere modificata.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="a7b1e-105">Di seguito sono riportati alcuni scenari in cui un file viene aperto in sola lettura e alcuni passaggi che è possibile eseguire per modificarlo.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="a7b1e-106">**Il mio antivirus sta facendo in modo che apra la sola lettura**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="a7b1e-107">Alcuni programmi antivirus possono proteggersi da file potenzialmente non sicuri aprendoli di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="a7b1e-108">Potrebbe essere necessario verificare con il provider di servizi antivirus per informazioni su come modificare queste impostazioni.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="a7b1e-109">BitDefender, ad esempio, ha contenuto per l'aggiunta di esclusioni di applicazioni qui: [come aggiungere esclusioni di applicazioni o processi nel centro di controllo di BitDefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="a7b1e-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="a7b1e-110">**Le proprietà del file sono impostate come di sola lettura?**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="a7b1e-111">È possibile controllare le proprietà del file facendo clic con il pulsante destro del mouse sul file e scegliendo Proprietà.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="a7b1e-112">Se l'attributo di sola lettura è selezionato, è possibile deselezionarlo e fare clic su OK.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="a7b1e-113">**Il contenuto è in visualizzazione protetta**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="a7b1e-114">I file provenienti da Internet e da altri percorsi potenzialmente non sicuri possono contenere virus, worm o altri tipi di malware che possono danneggiare il computer.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="a7b1e-115">Si tratta in genere anche degli allegati di posta elettronica o dei file scaricati.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="a7b1e-116">Per proteggere il computer, i file provenienti da questi percorsi potenzialmente non sicuri vengono aperti in visualizzazione protetta.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="a7b1e-117">Se si utilizza la visualizzazione protetta, è possibile leggere un file e visualizzarne il contenuto riducendo i rischi.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="a7b1e-118">Per ulteriori informazioni sulla visualizzazione protetta e su come modificare le impostazioni, vedere questo articolo: [che cos'è protectEd View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="a7b1e-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="a7b1e-119">**OneDrive è completo?**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="a7b1e-120">Se il file è archiviato su OneDrive e lo spazio di archiviazione di OneDrive è pieno, non sarà possibile salvare il documento finché non si è sotto lo spazio assegnato.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="a7b1e-121">È possibile controllare lo spazio disponibile su OneDrive facendo clic sull'icona di OneDrive nel centro notifiche e scegliendo Gestisci archiviazione oppure è possibile [http://onedrive.live.com](http://onedrive.live.com)accedere a, accedere e annotare la quantità di spazio utilizzato in basso a sinistra dello schermo.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="a7b1e-122">**Office è attivato?**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="a7b1e-123">Se Office non è attivato o se l'abbonamento è scaduto, è possibile che si trovi in modalità di sola lettura con funzionalità riDotte.</span><span class="sxs-lookup"><span data-stu-id="a7b1e-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="a7b1e-124">Per informazioni su come attivare Office, vedere: [errori di attivazione e di prodotto senza licenza in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="a7b1e-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="a7b1e-125">**Se tutto il resto ha esito negativo...**</span><span class="sxs-lookup"><span data-stu-id="a7b1e-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="a7b1e-126">Provare a riavviare il computer</span><span class="sxs-lookup"><span data-stu-id="a7b1e-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="a7b1e-127">Installare gli aggiornamenti di Office</span><span class="sxs-lookup"><span data-stu-id="a7b1e-127">Install Office updates</span></span>
    
- <span data-ttu-id="a7b1e-128">Eseguire un ripristino online di Office</span><span class="sxs-lookup"><span data-stu-id="a7b1e-128">Perform an Online repair of Office</span></span>
    

