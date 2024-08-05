---
title:  "How to send large audio files"
category: tutorial
tags: [share-file]
---
> As a hobby music producer, I often needed to share large WAVs, but existing services didn't really do it for me. Discord's 50MB limit was frustrating, and Google Drive, MEGA, Dropbox etc. felt cumbersome [...]. I rarely need to save my transfered files permanently, I just want to transfer them, and I think many others do too.

This quote is taken from the [GitHub page](https://github.com/robinkarlberg/transfer.zip-web/) of [Transfer.zip](https://transfer.zip/), and open source file sharing website that offers **unlimited file size** for free. The creator says that music production is their hobby, and uses the website to share large audio files (WAVs and MP3s) with friends or even potential clients.

**You may ask,** how can it be unlimited for free? 

Well, what makes TransferZipspecial is that the files are **never stored anywhere** on the servers, meaning the data is transfered directly between you and the recipient. This means there is no limit on how big the files can be, they are just sent over the air directly. 

The only caveat is that your browser window needs to be open during the whole file transfer, which is not a limitation in most scenarios: **it may be a good compromise to keep your browser window open for a couple of minutes, in return for free unlimited file transfer.**

## How to use transfer.zip

Using the service is easy, [navigate to transfer.zip](https://transfer.zip/) and press "Pick files" if you want to select individual files, or press "select a folder" to share all files stored in a specific folder. 

> When transfering a folder, it will be automatically converted to a .zip file in the browser, retaining the same directory structure and file names as in the original, when downloaded.
{: .prompt-tip }

![Screenshot showing the Quick Share page, a big QR code and a link to download the files.](/assets/img/quick-share-progress-1.png)
_Upon pressing Send, Quick Share will display a QR code and a link to copy._

To send the files, you can either let them scan the QR Code or, if they can't do that, you can send them a shareable link. Pressing the *copy to clipboard* button to the right of the link, copies the shareable link and you can send it to your recipient. 

When they visit the link, your devices will try to connect directly to each other using an encrypted connection with a secret key embedded in the link. Be patient, as large files can take time and depend on both you and your recipients network connection.

## Conclusion / Help

Using TransferZipis a game-changer for anyone needing to send large audio files or any other large files quickly and efficiently. The process is streamlined and user-friendly, making it accessible even for those who may not be tech-savvy.

If you encounter any issues or have questions while using transfer.zip, [submit an issue on their github page](https://github.com/robinkarlberg/transfer.zip-web) or send an email to [support@transfer.zip](mailto:support@transfer.zip).