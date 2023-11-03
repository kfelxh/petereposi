# Install Repositories on Linux

> Description:
> This is my personal guide to install Kali, Parrot and Kaisen repositories etc.


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
We create a **file with a .list extension**

```bash
```
