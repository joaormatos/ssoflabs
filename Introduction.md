# Lab1 - Introduction

The goal of this lab is to setup the course's laboratory environment and learn how to interact with a server using `pwntools` and `requests` modules from Python. Do not forget that in order to access our servers you should be connected to [IST VPN](https://si.tecnico.ulisboa.pt/servicos/redes-e-conetividade/vpn/).

## 1. Setup

1. Donwload the VM
    <!-- - Either the one we provide you [here](VM) or your favourite one -->
2. Install the VM (VirtualBox or VMWare Fusion)
3. Update the VM
    - `sudo apt update; sudo apt upgrade`
4. Register yourself in our [scoreboard](http://scoreboard.ssof.rnl.tecnico.ulisboa.pt) and start playing.

## 2. Learn how to use Python Requests - Challenge `Python requests`

During the course you will need to interact with our servers and a good way to do it is using package `requests` for Python.

    pip install requests (or pip3 install requests)

To practice we have prepared challenge `Python requests` in the scoreboard. The goal is simple: you are given a `target` number and you should access endpoint `/more` to get more numbers (randomly positive or negative) until the sum of all numbers is equal to `target`. Once you reach this value, you should access endpoint `/finish` to get the flag.

You can see [here](requests_template.py) a snippet on how to use module `requests`.

Notice that

- a) the start of the game is endpoint `hello`.
- b) the state is preserved using cookies so do not forget to send in a request the cookie that was received in the previous response.

Once you get the flag, submit it in our scoreboard to score points.

__Hints:__

- Are you being redirected to `/hello` when you request `/more`? See b) above.

## 3. Learn how to play with cookies - Challenge `Python requests Again`

Exercise `Python requests Again` is equal to the previous one but we only give you a chance to reach `target`. Can you do it?

## 4. Learn to use ZAP/Burp

To finalize this lab you can also use the previous exercise to learn how to use a Web Security Tool. You can chose between [OWASP ZAP (Zed Attack Proxy)](https://owasp.org/www-project-zap/) and [Burp Suite (Community Edition)](https://portswigger.net/burp/communitydownload).

In either case you will need to install a certificate in your browser so that these proxies can intercept and analyse your traffic. There are several tutorials available on how to do it ([for ZAP](https://www.zaproxy.org/docs/desktop/ui/dialogs/options/dynsslcert/#install)).

__Remarks:__ If you use the VM we provide, you should have to update the certificate. Take this chance and also update ZAP to its latest version.

## 5. Learn how to use sockets with pwntools - Challenge `PwnTools Sockets`

_You can postpone this one until you finish the Web Security labs_

During the course you will need to interact with our servers via sockets and a good way to do it is using package `pwntools` for Python.

    pip install pwntools (or pip3 install pwntools)

To practice we have prepared challenge `PwnTools Sockets` in the scoreboard. This exercise is the same game as `Python requests` but now over sockets. Instead of accessing endpoint `/more` you should send command `MORE`, and instead of accessing endpoint `/finish`, you should send command `FINISH`.

You can see [here](netcat_template.py) a snippet on how to use sockets in pwntools.

---

## Troubleshooting

- If you have problems installing `pwntools` with `pip3` just update pip3

      sudo python3 -m pip uninstall pip && sudo apt install python3-pip --reinstall
