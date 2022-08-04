# At Home With The GitOps

<img align="right" width="100" height="100" src="http://www.fillmurray.com/100/100">

Let me and Bill Murray show you our home GitOps setup. 

![Media server has rebooted on schedule](https://healthchecks.io/badge/37a7ad4c-57bd-4cea-9118-f2c5df/Qx0Lc7eg-2/mediaserver-regular-reboot.svg)
![Home Automation server has rebooted on schedule](https://healthchecks.io/badge/37a7ad4c-57bd-4cea-9118-f2c5df/i3csSel2-2/homeautomation-regular-reboot.svg)


- **Configuration as code:** `true`
- **Networking:** DHCP and DNS via Ansible-configured Pihole (though OPNsense soon to replace Pihole and the [Linksys Edge Router](ansible/inventory/host_vars/device-linksys-wrtacm3200.yaml)).
- **Hardware management:** all machines controlled via [Ansible](ansible).
- **Virtual machines:** provisioned via Terraform.
- **Container orchestration:** [Flux](flux) (but not for long) and Kubernetes, running on the provisioned VMs.

I started out writing this as a series of notes but it's growing into a mini-opera composed of weird sentence structures and addressing a constantly switching audience. I shall one day address this issue.

The majority of this repo is configuration code. But in `docs` there's a lot about the hardware and the reasons for my decisions. [View the docs directly in this repo](docs/) or [view the docs via a rendered site](https://whalecoiner.github.io/home/).

---

<details>
  <summary>:rotating_light: HUMAN EMOTION SECTION - DO NOT CLICK IF YOU DISLIKE FEELINGS :rotating_light:</summary>
  
## HUMAN EMOTION: PLEASE LEAVE IF YOU CAN'T COPE

This is all part of a huge learning and emotional experience for me. I spent a lot of 2020 and 2021 in hospital, dealing with a lot of medical shit. 
  
When I got out I decided that some changes were needed to my life. One of those changes was to make a gigantic (and frankly ill-planned) career change from Frontend Development - where I was mostly a manager and therefore spent my majority of time piloting spreadsheets -  right over to infrastructure & Platform Engineering as *an actual engineer and not a manager*.

Part of skilling up in this new role has been doing lots of learning on the side. 
  
This repo is one of those learnings. 
  
(Also I am coming to accept that I'm a massive nerd and that I'm allowed to play with tech shit as a hobby and that I probably have lots of internalised misogyny about a womans relationship to tech).

So if you see mistakes in this repo... well, it's because I'm new at all this. But on the bright side I think I'm coming into this strong and that things will only, as they say, get better. My enormous levels of ADHD (yes really ADHD and no not just being scatty) and me being a junior-grade space cadet means that my brain works well at fitting unrelated concepts and systems together. "Shit at the detail, fantastic at the big picture" is my elevator pitch. 

Anyway, enough of that. I'm sure you're hungry for code by now.

</details>


