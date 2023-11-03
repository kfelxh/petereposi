# Install Repositories on Linux

> Description:
> This is my personal guide to install Kali, Parrot and Kaisen repositories etc.

Note. This is my guide to installing Kali or Parrot repositories on Ubuntu or anything based on it. This guide is thanks to the support of @themasterx (Prof. Peter Xutuc) 🔭

[![Captura-de-pantalla-2023-11-03-002820.png](https://i.postimg.cc/43JDY0kV/Captura-de-pantalla-2023-11-03-002820.png)](https://postimg.cc/xX4x7td1)

<hr>

## Step 1 

*For this example I will install the Kali Linux repositories on Ubuntu*

[Kali Linux Repository](https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/ "www.kali.org")

[![Captura-de-pantalla-2023-11-03-063402.png](https://i.postimg.cc/pX2vbKYz/Captura-de-pantalla-2023-11-03-063402.png)](https://postimg.cc/ThHFnLs3)

## Step 2

Well, in my case I will install the repositories from the rolling branch. 

But the procedure is the same just with a different branch. You will have to investigate according to your need

[![Captura-de-pantalla-2023-11-03-063820.png](https://i.postimg.cc/rw1Y8HVp/Captura-de-pantalla-2023-11-03-063820.png)](https://postimg.cc/JshQxPBw)

>Observation: We just have to copy the repository.

***(Always consult the repository on the official Kali website as it is updated frequently.)***

```bash
deb http://http.kali.org/kali kali-rolling main contrib non-free non-free-firmware
```

## Step 3

Now, we head to the next route from our terminal.

```bash
cd /etc/apt/sources.list.d
```
Remember that we make these changes as a super user

```bash
sudo su 
```

We create a **file with a .list extension**

```bash
root@ubuntu:/etc/apt/sources.list.d$ mkdir kali.list
```
*Note: it doesn't matter what name you give the file, the only thing is that you can recognize it*

And paste the link to the kali repository

[![Screenshot-at-2023-11-03-15-42-02.png](https://i.postimg.cc/9fZdYC9b/Screenshot-at-2023-11-03-15-42-02.png)](https://postimg.cc/f3WSw4BS)


**I know, I'm a fan of the beautiful Nayeon. 😳**

We save the file.  And ready

<hr>

## Step 4

Now we have to sign it, for that we are heading to the same route

Now we have to sign, for that copy the link that is in the repository that is...

[http://http.kali.org/kali](http://http.kali.org/kali)

[![Captura-de-pantalla-2023-11-03-160019.png](https://i.postimg.cc/qqv6SCbJ/Captura-de-pantalla-2023-11-03-160019.png)](https://postimg.cc/MMgGjXJN)

**We're going to**
**And we download the *.deb* key file**

``http://http.kali.org/kali/pool/main/k/kali-archive-keyring/``

[![Captura-de-pantalla-2023-11-03-160210.png](https://i.postimg.cc/W3hh7Phz/Captura-de-pantalla-2023-11-03-160210.png)](https://postimg.cc/cgGxs27G)

## Step 5

We install the .deb file as we normally do

```bash
sudo apt install ./kali-archive-keyring_2022.1_all.deb
```

And

```bash
sudo apt update 
```

[![Captura-de-pantalla-2023-11-03-161154.png](https://i.postimg.cc/CKbvLWFZ/Captura-de-pantalla-2023-11-03-161154.png)](https://postimg.cc/DWyQxp4F)

We tried installing a Kali tool, for example Wireshark.

```bash
sudo apt install wireshark 
```

[![Captura-de-pantalla-2023-11-03-161455.png](https://i.postimg.cc/k4Xx3ZDP/Captura-de-pantalla-2023-11-03-161455.png)](https://postimg.cc/nsgsq3v3)

<hr>

## Finish

 And well that's all we have installed kali repositories in ubuntu debian or any distribution based on them

By *xutucluis* 🧊 <!--(@kfelxh)-->
([X @kfelxh](https://twitter.com/kfelxh "twitter"))
