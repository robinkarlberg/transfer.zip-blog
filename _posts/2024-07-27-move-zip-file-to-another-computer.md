---
title:  "Move zip file to another computer"
---
> Every time you email a file to yourself so you can pull it up on your friend's laptop, Tim Berners-Lee sheds a single tear.

That quite humorous quote is taken from [xkcd #949](https://xkcd.com/949/), a popular web comic depicting how hard file transfers can be, even on the modern web:

![xkcd depicting a file transfer being difficult](https://imgs.xkcd.com/comics/file_transfer.png)

But really, what is the easiest way to move a file from one computer to another? With a USB stick? Or set up an FTP server? Most likely, your USB stick is too slow and too small for your files, and setting up an FTP server requires you to be very technical. 

[transfer.zip](https://transfer.zip) is a service that hopes to solve all these problems, and best of all, **it is free and there is no size limit**. If you want to move, lets say a .ZIP file from one computer to another, [transfer.zip](https://transfer.zip) should be easier and work better than most alternatives like using USB sticks or mailing the file to yourself, or online services like WeTransfer and Dropbox.

## What is transfer.zip?

[transfer.zip](https://transfer.zip) is a file transfer website that prides itself by not requiring an account or any paid subscription to transfer files. It is open source, meaning that its source code is freely available for anyone to view, modify, and distribute. This openness allows for transparency, security, and community-driven improvements. Developers from around the world can contribute to the project, ensuring it remains reliable and up-to-date.

The quickest way to share files on transfer.zip is using *Quick Share*, the primary feature of the website. 

### How to use Quick Share

### **1. Go to the website and select your files**

To get started with Quick Share, head over to the official site at [transfer.zip](https://transfer.zip/). There, you can choose your files or even an entire folder if needed, that will be automatically zipped. After making your selection, the interface should display the file names in a designated area, resembling this example:

![Screenshot of Quick Share showing that the user has picked a 100GB file](/assets/img/quick-share-100g.png){: width="400"}

### **2. Press the send button**

After selecting your files, hit the Send button. This action will generate a large QR code and a button to copy a shareable link. The link provided is what the recipient will use to download the files. This link contains a unique identifier and a 256-bit encryption key that is created in your browser, ensuring that **transfer.zip can never access the encryption key.**

![Screenshot of Quick Share showing a big QR code and that the user is waiting for someone to scan it](/assets/img/quick-share-progress-1.png)

### **3. Scan the QR code or share the link**

Next, you can either let the other device scan the QR code if it is a phone, but if you want to send it to a computer you most likely need to send the link another way. You could mail the link to them, or send it on Discord, Facebook or Twitter. When the receiver scans the QR code or clicks the link, your devices will attempt to establish a peer-to-peer connection. Typically, this connection is made instantly, but if network firewalls block direct connections, the devices will not connect directly.

In such scenarios, Quick Share uses its servers to relay the encrypted file information. Even then, due to end-to-end encryption, **transfer.zip cannot access your files.**

### **4. Wait for the file transfer to complete**

Once connected, the file transfer begins. The transfer occurs in real-time, so if either party closes their browser tab or window, the transfer will halt and need to be restarted. This is a primary limitation of transfer.zip's Quick Share, but it allows for transferring extremely large files. The transfer speed depends on the internet connections of both parties, so large files might take a while. Please be patient!

![Screenshot of Quick Share showing the 100GB file is being downloaded](/assets/img/quick-share-progress-100g-3.png)

### **5. Completed!**

Thank you for using Quick Share by transfer.zip. We hope the file transfer was successful. If you encounter any issues, please [submit an issue on our GitHub page](https://github.com/robinkarlberg/transfer.zip-web/issues).
