---
layout: post
title:  "How to easily upload zip file with transfer.zip"
---
**Seemingly, there is no quick and easy way to upload and send files like .zip-files on the modern web.** You might start with WhatsApp, but its 16MB limit can be frustratingly restrictive. Email isn't feasible due to attachment size constraints. Dropbox looks promising, but it has a 2GB limit on free file transfers. OneDrive could be another option, but its interface is overly complex, **you just want something quick, easy and free!**

## Upload zip file with **[transfer.zip](https://transfer.zip/)**

[transfer.zip](https://transfer.zip/) is a free and [open source](https://github.com/robinkarlberg/transfer.zip-web) platform that allows you to send files of any size. The source code is available on GitHub [here](https://github.com/robinkarlberg/transfer.zip-web), offering transparency and the option to self-host for added security. The official version at [https://transfer.zip/](https://transfer.zip/) runs the same verified code from the GitHub repository, ensuring it's just as secure.

If you've struggled with uploading large zip files online, this service is worth trying. It stands out from other services, which can be both advantageous and disadvantageous, but it might be exactly what you need. The most notable feature is *Quick Share*, the primary function of the service, enabling the transfer of files of any size. 

### How to use transfer.zip to upload a zip file

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