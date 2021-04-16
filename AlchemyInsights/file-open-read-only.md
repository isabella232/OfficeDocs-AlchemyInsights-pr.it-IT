---
title: Apertura file di sola lettura
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813188"
---
# <a name="file-open-read-only"></a><span data-ttu-id="12d87-102">Apertura file di sola lettura</span><span class="sxs-lookup"><span data-stu-id="12d87-102">File open read-only</span></span>

<span data-ttu-id="12d87-103">È possibile che quando si aprono i file, questi vengono aperti in sola lettura.</span><span class="sxs-lookup"><span data-stu-id="12d87-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="12d87-104">In alcuni casi, ciò è per una sicurezza aggiunta, ad esempio quando si aprono file da Internet e altre volte, può essere dovuto a un'impostazione che può essere modificata.</span><span class="sxs-lookup"><span data-stu-id="12d87-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="12d87-105">Ecco alcuni scenari in cui un file viene aperto in sola lettura e alcuni passaggi che puoi eseguire per modificarlo.</span><span class="sxs-lookup"><span data-stu-id="12d87-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="12d87-106">**L'antivirus sta causando l'apertura di sola lettura**</span><span class="sxs-lookup"><span data-stu-id="12d87-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="12d87-107">Alcuni programmi antivirus potrebbero proteggere l'utente da file potenzialmente non sicuri aprendoli di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="12d87-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="12d87-108">Potrebbe essere necessario rivolgersi al provider antivirus per informazioni su come modificare queste impostazioni.</span><span class="sxs-lookup"><span data-stu-id="12d87-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="12d87-109">BitDefender, ad esempio, include contenuto sull'aggiunta di esclusioni di applicazioni qui: Come aggiungere le esclusioni di applicazioni o processi nel Centro di controllo [Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="12d87-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="12d87-110">**Le proprietà del file sono impostate come di sola lettura?**</span><span class="sxs-lookup"><span data-stu-id="12d87-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="12d87-111">È possibile controllare le proprietà del file facendo clic con il pulsante destro del mouse sul file e scegliendo Proprietà.</span><span class="sxs-lookup"><span data-stu-id="12d87-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="12d87-112">Se l'attributo di sola lettura è selezionato, è possibile deselezionarlo e fare clic su OK.</span><span class="sxs-lookup"><span data-stu-id="12d87-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="12d87-113">**Il contenuto è in visualizzazione protetta**</span><span class="sxs-lookup"><span data-stu-id="12d87-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="12d87-114">I file provenienti da Internet e da altri percorsi potenzialmente non sicuri possono contenere virus, worm o altri tipi di malware che possono danneggiare il computer.</span><span class="sxs-lookup"><span data-stu-id="12d87-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="12d87-115">Questo è in genere anche il caso degli allegati di posta elettronica o dei file scaricati.</span><span class="sxs-lookup"><span data-stu-id="12d87-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="12d87-116">Per proteggere il computer, i file da questi percorsi potenzialmente non sicuri vengono aperti in Visualizzazione protetta.</span><span class="sxs-lookup"><span data-stu-id="12d87-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="12d87-117">Utilizzando Visualizzazione protetta, è possibile leggere un file e visualizzarne il contenuto riducendo al contempo i rischi.</span><span class="sxs-lookup"><span data-stu-id="12d87-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="12d87-118">Per ulteriori informazioni su Visualizzazione protetta e su come modificare le impostazioni, vedere questo articolo: [Che cos'è Visualizzazione protetta?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="12d87-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="12d87-119">**OneDrive è pieno?**</span><span class="sxs-lookup"><span data-stu-id="12d87-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="12d87-120">Se il file è archiviato in OneDrive e lo spazio di archiviazione di OneDrive è pieno, non sarà possibile salvare il documento finché non si è sotto lo spazio assegnato.</span><span class="sxs-lookup"><span data-stu-id="12d87-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="12d87-121">È possibile controllare lo spazio disponibile in OneDrive facendo clic sull'icona OneDrive nel centro notifiche e scegliendo Gestisci spazio di archiviazione oppure è possibile passare a , accedere e prendere nota della quantità di spazio usato in basso a sinistra dello [https://onedrive.live.com](https://onedrive.live.com) schermo.</span><span class="sxs-lookup"><span data-stu-id="12d87-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="12d87-122">**Office è attivato?**</span><span class="sxs-lookup"><span data-stu-id="12d87-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="12d87-123">Se Office non è attivato o se l'abbonamento è scaduto, è possibile che si sia attivata la modalità a funzionalità ridotte di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="12d87-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="12d87-124">Per informazioni su come attivare Office, vedere: Errori di attivazione e prodotti senza [licenza in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="12d87-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="12d87-125">**Se tutto il resto ha esito negativo...**</span><span class="sxs-lookup"><span data-stu-id="12d87-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="12d87-126">Provare a riavviare il computer</span><span class="sxs-lookup"><span data-stu-id="12d87-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="12d87-127">Installare gli aggiornamenti di Office</span><span class="sxs-lookup"><span data-stu-id="12d87-127">Install Office updates</span></span>
    
- <span data-ttu-id="12d87-128">Eseguire un ripristino online di Office</span><span class="sxs-lookup"><span data-stu-id="12d87-128">Perform an Online repair of Office</span></span>
    

