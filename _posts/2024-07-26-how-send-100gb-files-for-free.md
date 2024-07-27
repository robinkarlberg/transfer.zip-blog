---
layout: post
title:  "How to send 100GB files for free"
---
**Everyone has faced challenges when trying to send big files online.** First, you might attempt to send it via Discord, only to discover that it has a 25MB limit. Email isn't a viable option either due to its size restrictions. Uploading to WeTransfer seems like a solution, but it caps at 2GB. Google Drive could work, but you find it to be cluttered with too many buttons and options, you also know that Google happily steals your data to sell to the highest bidder. 

<!-- ...so enter transfer.zip: -->

## No file size limit for free with **[transfer.zip](https://transfer.zip/)**

[transfer.zip](https://transfer.zip/) is a free and [open source](https://github.com/robinkarlberg/transfer.zip-web) project that actually enables you to send files **as large as you want**. The source code is hosted on GitHub [here](https://github.com/robinkarlberg/transfer.zip-web), and to build ultimate trust, it features a self-hosting mode so you can host it yourself, to be sure that no one peeks on your files. However, the official version at [https://transfer.zip/](https://transfer.zip/) is running the same verifiable code as in the GitHub repository, so it is just as safe.

If you have had problems sending large files over the internet, you should give it a try, because this service is not like the others, which is both good and bad, but may be exactly what you are looking for. The most useful feature is called *Quick Share*, and is the primary feature of the service, which enables you to send files of any size. The GitHub page explains the technical details behind it:

> Quick Share uses WebRTC for peer-to-peer data transfer, meaning the files are streamed directly between peers and not stored anywhere in the process, not even on transfer.zip servers. To let peers initially discover each other, a signaling server is implemented in NodeJS using WebSockets, which importantly no sensitive data is sent through. In addition, the file data is end-to-end encrypted using AES-GCM with a client-side 256 bit generated key, meaning if someone could impersonate a peer or capture the traffic, they would not be able to decrypt the file without knowing the key. Because the file is streamed directly between peers, there are no file size or bandwidth limitations.

To summarize, Quick Share uses a peer-to-peer connection without server storage, which means files are not stored and thus can be as large as you want. Files are end-to-end encrypted and streamed in real-time from the sending device to the receiving device.

### How to use Quick Share

#### **1. Visit the website and pick your files**

To use Quick Share, just navigate to the official website at [transfer.zip](https://transfer.zip/). There you will be instructed to pick your files, or pick a whole folder if that's your thing. Once the files are picked, it should look something like this, with the file name appearing in the file box:

<!-- ![Quick Share landing page](/assets/img/quick-share-new.png){: width="400"} -->
![Screenshot of Quick Share showing that the user has picked a 100GB file](/assets/img/quick-share-100g.png){: width="400"}

#### **2. Click send**

Once you have picked your files, click the Send button, and it will show you a big QR code and a button to copy the shareable link. The shareable link is the URL that the receiver should visit to download the file. The shareable link contains a unique identifier for your files, along with a 256-bit encryption key that was generated locally in your browser, meaning **transfer.zip never has access to the encryption key.**

![Screenshot of Quick Share showing a big QR code and that the user is waiting for someone to scan it](/assets/img/quick-share-progress-1.png)

#### **3. Scan the QR code or share the link**

Now, you have the option to either let them scan the QR Code, or if they are unable to, you can send them the shareable link. As soon as they scan the QR code or click the link, your devices will try to set up a peer-to-peer connection to each other. In most cases that will work and the devices will connect instantly, but sometimes network firewalls may disallow such direct connections, which means the devices will not be able to connect directly. 

In such cases, Quick Share relays the encrypted file information through one of its servers. As the files are end-to-end encrypted, **it is still impossible for transfer.zip to read the files.**

#### **4. Wait while the files are being transfered**

Finally, when the connection is established, the files will begin transferring. Remember that they are transfered in real-time, so if anyone closes their browser tab or window, the transfer will be stopped and will need to be restarted again. This is one of the biggest limitations of transfer.zip's Quick Share, but it is also the reason why the files can be so infinitely large. The transfer speed is limited by your and your receivers internet connection, so sending big files could take time. Be patient!

![Screenshot of Quick Share showing the 100GB file is being downloaded](/assets/img/quick-share-progress-100g-3.png)

#### **5. Done!**

transfer.zip thanks you for using our Quick Share service, hopefully the file transfer went smoothly. If you encounter any problems, please [submit an issue at our GitHub page](https://github.com/robinkarlberg/transfer.zip-web/issues).