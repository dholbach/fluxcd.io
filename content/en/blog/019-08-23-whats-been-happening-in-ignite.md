---
author: dholbach
date: 2019-08-23 17:49:43+00:00
draft: false
title: What's been happening in Ignite
type: posts
comments: true
url: /blog/2019/08/whats-been-happening-in-ignite/
images:
- /images/2019/08/logo.png
categories:
- OpenSource
- Weaveworks
tags:
- firecracker
- gitops
- weave ignite
---





_First of all: thanks [Dennis Marttinen](https://github.com/twelho) and [Lucas Käldström](https://github.com/luxas) for helping write this up._







It’s been only a bit over a month since [Weave Ignite was announced to the world](https://www.weave.works/blog/fire-up-your-vms-with-weave-ignite) ([others](http://arun-gupta.github.io/ignite-firecracker/) [talked](https://blog.kubernauts.io/ignite-on-google-cloud-5d5228a5ffec) [about](https://www.youtube.com/watch?v=aq-wlslJ5MQ) [it](https://thenewstack.io/weave-ignite-brings-a-container-gitops-experience-to-vms/) [as](https://felixwiedmann.de/ignite/) [well](https://www.techrepublic.com/article/the-clearest-sign-of-aws-open-source-success-wasnt-built-by-amazon)). Time to catch up on what happened in the meantime, the team around it has been busy.  








If you’re new to [Weave Ignite](https://github.com/twelho), it’s an open source VM manager with a container UX and built-in GitOps management (check out the [docs](https://ignite.readthedocs.org)). It’s built on top of [Firecracker](https://firecracker-microvm.github.io/) which has proven to be able to run[ 4000 micro-VMs on the same host](https://github.com/firecracker-microvm/firecracker-demo). Time to [give it a go](https://ignite.readthedocs.io/en/stable/installation.html), right?  








Since the initial announce 43 people contributed to the project on Github, 20 got commits merged in the repo. Thanks to every one of you:   








[@BenTheElder](https://github.com/BenTheElder),[ @DieterReuter](https://github.com/DieterReuter),[ @PatrickLang](https://github.com/PatrickLang),[ @Strum355](https://github.com/Strum355),[ @akshaychhajed](https://github.com/akshaychhajed),[ @alex-leonhardt](https://github.com/alex-leonhardt),[ @alexeldeib](https://github.com/alexeldeib),[ @alexellis](https://github.com/alexellis),[ @andrelop](https://github.com/andrelop),[ @andrewrynhard](https://github.com/andrewrynhard),[ @aojea](https://github.com/aojea),[ @arun-gupta](https://github.com/arun-gupta),[ @asaintsever](https://github.com/asaintsever),[ @chanwit](https://github.com/chanwit),[ @curx](https://github.com/curx),[ @danielcb](https://github.com/danielcb),[ @dholbach](https://github.com/dholbach),[ @hbokh](https://github.com/hbokh),[ @jiangpengcheng](https://github.com/jiangpengcheng),[ @junaid18183](https://github.com/junaid18183),[ @kim3z](https://github.com/kim3z),[ @liwei](https://github.com/liwei),[ @luxas](https://github.com/luxas),[ @najeal](https://github.com/najeal),[ @neith00](https://github.com/neith00),[ @paavan98pm](https://github.com/paavan98pm),[ @patrobinson](https://github.com/patrobinson),[ @pditommaso](https://github.com/pditommaso),[ @praseodym](https://github.com/praseodym),[ @prologic](https://github.com/prologic),[ @robertojrojas](https://github.com/robertojrojas),[ @rugwirobaker](https://github.com/rugwirobaker),[ @saiyam1814](https://github.com/saiyam1814),[ @seeekr](https://github.com/seeekr),[ @sftim](https://github.com/sftim),[ @silenceshell](https://github.com/silenceshell),[ @srinathgs](https://github.com/srinathgs),[ @stealthybox](https://github.com/stealthybox),[ @taqtiqa-mark](https://github.com/taqtiqa-mark),[ @twelho](https://github.com/twelho),[ @tyhal](https://github.com/tyhal),[ @vielmetti](https://github.com/vielmetti),[ @webwurst](https://github.com/webwurst)  








Since then the team got [four releases](https://github.com/weaveworks/ignite/releases/) out the door. Let’s go through the big changes one by one and why they matter:  






  * Lots of bug fixes, enhanced stability, more tests and more and better docs ([find them here](https://ignite.readthedocs.io/))
  * Support for Persistent Storage, ARM64, manifest directories, the improved _v1alpha2 API,_ both declarative and imperative VM management
  * More pre-built VM images (currently there are images based on Ubuntu, CentOS, Amazon Linux, Alpine and OpenSUSE + a kubeadm image)
  * _ignited_ was introduced to move Ignite towards a client-server model and improve VM lifecycle management
  * The Docker-like UX has been further improved, now also featuring ‘ignite exec’
  * Read-write GitOps support, now status updates/changes (e.g. IP addresses) are pushed back to the repository





It’s impressive how such a young project got all of this together in such a short amount of time (only around a month).







  
We also have been busy growing our community. As mentioned above, [documentation](https://ignite.readthedocs.org) was an important part of this: [API docs](https://ignite.readthedocs.io/en/stable/api/ignite_v1alpha2.html), a very solid [CLI reference](https://ignite.readthedocs.io/en/stable/cli/ignite/index.html) and [short](https://ignite.readthedocs.io/en/stable/usage.html) [tutorials](https://ignite.readthedocs.io/en/stable/declarative-config.html) to get you started were the key.  








We also started a mailing list and regular community Ignite developer meetings. These happen Mondays at 15:00 UTC ([what’s UTC?](https://www.timeanddate.com/worldclock/timezone/utc)) and are meant to get people together who are generally interested in Ignite and want to learn more and potentially help out as well. Project authors [Lucas Käldström](https://github.com/luxas) and [Dennis Marttinen](https://github.com/twelho) are always very approachable, but here especially they made a point of introducing everyone to the goals behind Ignite, its [roadmap](https://ignite.readthedocs.io/en/stable/roadmap.html) and the currently ongoing work.  








We’ve recorded [all of the meetings](https://www.youtube.com/playlist?list=PLbx4FZ4kOKnuD4gkjk7SHaJAALw7yWG0U). [Meeting Notes](https://docs.google.com/document/d/1fv8_WD6qXfvlIq7Bb5raCGyBvc42dNF-l8uaoZzoUYI/edit) are available too (Please join [weaveworks-ignite](https://groups.google.com/forum/#!forum/weaveworks-ignite) on Google Groups to get write access).  








Here’s what we covered so far:  






  * [1st meeting](https://www.youtube.com/watch?v=H8aUCqQipEs&list=PLbx4FZ4kOKnuD4gkjk7SHaJAALw7yWG0U&index=2&t=0s):
    * Team introductions
    * Demo of Ignite
    * Roadmap overview
    * Current work-in-progress
  * [2nd meeting](https://www.youtube.com/watch?v=1qmIb7xMc98&list=PLbx4FZ4kOKnuD4gkjk7SHaJAALw7yWG0U&index=3&t=0s):
    * What’s coming in v0.5.0?
    * Roadmap for v0.6.0
    * Integration with Kubernetes through Virtual Kubelet
    * How to contribute to Ignite
  * [3rd meeting](https://youtu.be/Sv9lOYDZrFo)
    * v0.5.0 and v0.5.1 released
    * GitOps Toolkit is being split out - what is it for?
    * Footloose integration - what is it about?
    * Coming up: containerd support
    * Discussion of application logging





And this is where you come in… our next meeting is **Monday, 26th August 2019 15:00 UTC** and we have an action packed [agenda](https://docs.google.com/document/d/1fv8_WD6qXfvlIq7Bb5raCGyBvc42dNF-l8uaoZzoUYI/edit) as well:  






  * containerd integration
  * CNI integration
  * The GitOps Toolkit
  * Code walk-through / project architecture
  * Discussion: what would you like to see in Ignite? What do/could you use it for?
  * Releasing v0.6.0
  * <you can still add your own agenda item [here](https://docs.google.com/document/d/1fv8_WD6qXfvlIq7Bb5raCGyBvc42dNF-l8uaoZzoUYI/edit)>





We are very excited to see the direction Ignite is taking, particularly because it contributes a lot to the ecosystem. How?  








We realised that all the GitOps functionality of Ignite would be useful to the rest of the world, so we split it out into the [GitOps Toolkit](https://github.com/weaveworks/gitops-toolkit).  








The team is also working on _containerd_ integration, so that you don’t need Docker installed to run Ignite VMs. Why does Ignite require a container runtime to be present? Because Ignite integrates with the container world, so you can seamlessly run both VMs and containers next to each other. containerd is super lightweight, as is Firecracker, so pairing them with Ignite makes a lot of sense!  








If the above sounds exciting to you and your project, please share the news and meet up with us on Monday. We look forward to seeing you there!  








But that’s not all. This is just where we felt Ignite could make a difference. If you have your own ideas, own use-cases, issues or challenges, please let us know and become part of the team - even if it’s just by giving us feedback! If you’d like to get inspiration about what others are doing with Ignite, or add your own project, check out the [awesome-ignite](https://ignite.readthedocs.io/en/stable/awesome.html) page.  








If you are interested in helping out, that’s fantastic! The meeting should be interesting for you too. If you can’t wait, check out our [contributors guide](https://github.com/weaveworks/ignite/blob/master/CONTRIBUTING.md) and check out our [open issues](https://github.com/weaveworks/ignite/issues) too. If you are interested in writing docs, adding comments, testing, filing issues or getting your feet into the project, we’re all there and happy to help.  








We’ll have more news on Ignite soon. But for today’s update we are signing off with a bitter-sweet announcement: Lucas and Dennis will from September step down as project maintainers in order to embark on a new adventure: [Aalto University](https://www.aalto.fi/en) in Helsinki! They have started something very remarkable and we could not be happier for them. Watch this space for more news.







If you’d like to join the journey, you can do so here:  






  * [Get started with Ignite](https://ignite.readthedocs.io/)
  * Check out the [demo in the video](https://www.youtube.com/watch?v=s_O75zt-oBg)
  * Join us **Monday, 26th August 2019 15:00 UTC** in the next [Ignite Dev meeting](https://docs.google.com/document/d/1fv8_WD6qXfvlIq7Bb5raCGyBvc42dNF-l8uaoZzoUYI/edit).

