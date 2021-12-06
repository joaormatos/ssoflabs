# Labs of Software Security Course@IST

Welcome to the Software Security Course@IST Labs! Please read this page until the end before you start.

This repo is permanently under construction and the goal is to provide you with tips for solving the challenges as well as with pointers for studying more. If you find something wrong, some topic that needs to be updated/added, please create an issue on that topic.

Follow the links below devoted to each topic. __The links that are marked (2020/21) have not yet been updated for the current semester (Fall 2021/22).__

The goal for these labs of Software Security is that you learn by doing, and for that you should try hard. In each lab you'll be challenged with 3 to 4 different vulnerable challenges associated with a given topic. In some cases, these challenges will then be patched and a more powerfull technique will have to be applied in order to solve the updated version of the challenge.

And there will be a competition during the whole semester!

But first things first.

__Never run potential malicious content in your machine. You must install a VM as a basic form of sandboxing.__

## 1. Install Tecnico VPN

In order to play these challenges, access the scoreboard, and download the VM you have to be connected to the IST VPN. __It is not enough to be on campus.__ You can find the instructions on how to connect to the VPN [here](https://si.tecnico.ulisboa.pt/servicos/redes-e-conetividade/vpn/).

## 2. Virtual Machines 

__Never run potential malicious content in your machine. You must install a VM as a basic form of sandboxing.__

(OUTDATED)

You must have a VM with the appropriate tools installed. You can pick your preferred distribution, or use the one we provide you [here](https://storage.ssof.rnl.tecnico.ulisboa.pt/).

    SHA1SUM (ubuntu_ssof.ova): 391a9de81f4c8a4f729a8380a9edddc340b8a8eb

It is a Ubuntu 18.04.1 VM and we hope you have in there everything you need for this course. It was created for the school year 2018/19 so the first thing to do after importing it is

    sudo apt update; sudo apt upgrade

More details about installing instructions, login details, list of installed software, and troubleshooting can be found [here](VM.md).

## 3. Scoreboard

This year's labs we will have a [scoreboard](https://scoreboard.ssof.rnl.tecnico.ulisboa.pt/) where you should submit the solutions for your challenges. You need a `@tecnico.ulisboa.pt` or `@ist.utl.pt` e-mail in order to register. If you do not have one, please [contact us](mailto:pedro.adao@tecnico.ulisboa.pt). __Do not use an important password for this scoreboard.__

All challenges will run on machine `mustard.stt.rnl.tecnico.ulisboa.pt`. Each challenge will run on a specific port that will be given to you as part of the challenge.

Flags will be of the form `SSof{....}` unless otherwise explicitly stated. Once you solve a challenge and find a flag, you can submit it in our scoreboard to score points.

Although there is no evaluation for these labs, this competition will last the whole semester and there could be prizes for top-3 performers.

GOOD LUCK!

## 4. Links

- [SSof Scoreboard](https://scoreboard.ssof.rnl.tecnico.ulisboa.pt/)
- [Virtual Machine Details](VM.md)
- Basic usage of tools
  - [Using Burp Suite as a Web Proxy](Burp.md) (2020/21)
  - [gdb Basics](GDB.md) (2020/21)
- Labs
  - [Lab1 - Introduction](Introduction.md)
  <!-- - [Lab2 - Race Conditions](RaceConditions.md) -->
  <!-- - [Lab3 - Buffer Overflows](BufferOverflows.md) -->
  <!-- - [Lab4 - Format Strings](FormatStrings.md) -->
  <!-- - [Lab5 - Cross Site Scripting (XSS)](XSS.md) -->
  <!-- - [Lab5 - Cross Site Request Forgery (CSRF)](CSRF.md) -->
  <!-- - [Lab6 - SQL Injection](SQLi.md) -->
  - Still to be updated for the current year
    - All done
