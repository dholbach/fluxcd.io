---
author: dholbach
date: 2020-03-02 10:15:55+01:00
draft: false
title: 2 Years at Weaveworks
type: posts
comments: true
url: /blog/2020/03/2-years-at-weaveworks/
images:
- /images/2018/02/logo_weaveworks.png
categories:
- OpenSource
- Weaveworks
tags:
- weaveworks
- gitops
- oss
- k8s
- cloudnative
---

Time flies when you're having fun: it's now been [two years](/blog/2018/02/im-joining-weaveworks/) since I started working at Weaveworks and I 💕 the experience it's been.

Back then I was just concluding [my sabbatical](/blog/2018/02/took-a-year-off/) and had started pursuing a second career in that year. So my mind wasn't exactly in the tech space, still I felt rested and open to new challenges. In the meantime, many old friends had already waved over from Cloud Native land and tried to lure me there. Especially my [ex team mate Jorge Castro](https://twitter.com/castrojo) had raved  about the Kubernetes community whenever we talked: that future was being made here and that the people were great and this was exactly the right thing to be involved with. If you know him just a little bit, you know this is typical Jorge.

When I set out looking for a job, I was lucky that [Jono Lange](https://jml.io/) reached out as well and told me what was happening at Weave. A couple of weeks later I was part of the team. The interview process was great because I got to talk to lots of people and get a feel for the entire team and their vision. The process wasn't without mishaps though: to [Alexis](https://twitter.com/monadic) I talked on a video call out of a car on a mountain on Euboea, Greece - it was the only place where I had passable reception, to a call with [Tamao](https://twitter.com/mewzherder) I was 20 minutes late because of traffic in Cairo - ouch! - and when I talked to Matthias, [Ilya](https://twitter.com/errordeveloper) and [Stefan](https://twitter.com/stefanprodan) I had turn off video at times because the internet in Dahab at the Red Sea wasn't quite up to it. I'm so glad they came to the conclusion to have me as part of the team and my future team put up with this.

I was a bit weary starting into this, since I had been out of tech for 13 months and the Cloud Native landscape is simply overwhelming when you're new: it is a HUGE community, a big entangled mess of competing solutions, vendors, tools, its own lingo, hundreds of sub-communities and challenges I hadn't deeply considered yet. Frankly, it was a very daunting perspective at the time and I wasn't sure if I could "learn all of this" - in my mind, that's what I thought I needed to do.

What helped me ease into the job and communities were right from the start my teams: [Bianca](https://twitter.com/rhizop), [Filip](https://github.com/fbarl), [Lili](https://twitter.com/LiliCosic) and [Simon](https://github.com/foot) in Berlin and the DX gang: Tamao, Ilya, Stefan, [Lucas](https://twitter.com/kubernetesonarm), [Leigh](https://twitter.com/capileigh), [Stacey](https://twitter.com/stacey_potter), [Dennis](https://twitter.com/twelho) and [Chanwit](https://twitter.com/chanwit).

All of them were infinitely patient, had great ideas to help me grow, encouraged me to dig deeper, introduced me to other interesting folks and gave me the feeling that even if they would probably never let me go near Prod or a customer's cluster, that I was generally doing an all right job finding into this space. 🙏

My immediate impression from Weaveworks was that I enjoyed the fact that the company was smaller than Canonical (where I worked before) a lot: getting things done across "departments" (I think we were around 25 people when I joined) was often an ad-hoc affair that often just involved a call or chat on Slack. It gave me a sense of being able to influence direction and that people generally trusted my judgement. As the token German in my teams I sometimes felt things could be a bit more structured, so I was happy to help e.g. putting together a Wiki from our internal docs, setting up a Knowledge Base and so on.

There were so many things I got to work on and folks I collaborated with. Particularly that there is so much Open Source in our story makes me proud and happy to be here. Here are a few of my highlights:

Supporting our booth and workshops at conferences was fun! It got me in touch with many of our users, customers and friends - I learned a lot about the field and everyone's challenges there.

I spent quite some time with the [Flux](https://fluxcd.io/) team ([Michael](https://github.com/squaremo), Stefan, [Hidde](https://twitter.com/hiddeco), [Fons](https://twitter.com/2opremio)). As one of our most important projects, making Flux [more accessible to users](https://www.weave.works/blog/install-fluxctl-and-manage-your-deployments-easily) and developers was very rewarding. Initiatives like [simplifying installation](https://docs.fluxcd.io/en/stable/tutorials/get-started.html), [adding more docs](https://docs.fluxcd.io/), improving [some of the community structures](https://www.weave.works/blog/weave-increased-our-flux-capacity) fell on very fertile ground: the number of users and contributors exploded over time. [Flux entering the CNCF](https://www.weave.works/blog/flux-joins-the-cncf-sandbox) was probably another big contributing factor. [Flux and Argo joining forces](https://www.weave.works/blog/argo-flux-join-forces) is just another big milestone on the way.

Working with the [Scope](https://github.com/weaveworks/scope) team (Fons, [Bryan](https://twitter.com/bboreham), Filip, [Satyam](https://twitter.com/SatyamZode), [Akash](https://github.com/qiell)) was a lot of fun too. It's still one of the most loved k8s projects out there, you see it at booths and in workshops a lot, so having a healthy group maintaining it and [re-integrating features](https://www.weave.works/blog/never-lose-data-with-persistent-volume-snapshots-in-weave-scope-1-10) from [experiments elsewhere](https://www.weave.works/blog/troubleshoot-your-cluster-from-visual-studio-code-with-weave-scope) was important. [Visiting Satyam and Akash](https://www.weave.works/blog/mayadata-brings-data-agility-to-customers-using-weave-scope) and the entire MayaData team in Bangalore and working with them was a great experience too. Miss the great food there too!

During my time at Weave we released many useful tools to the world, all open source. If you haven't checked out [Firekube](https://github.com/weaveworks/wks-quickstart-firekube), [Ignite](https://github.com/weaveworks/ignite), [Footlose](https://github.com/weaveworks/footloose), [eksctl](https://eksctl.io), [wksctl](https://github.com/weaveworks/wksctl), [Flagger](https://flagger.app) or any of the other good stuff yet, please do - they're going to make your life easier! I was happy to be able to help out in putting open source, community and docs structures in place for them. I recently helped others breath new life into [kured](https://github.com/weaveworks/kured) and [grafanalib](https://github.com/weaveworks/grafanalib) - stay tuned for contributors meetings for the two any time soon.

I also started contributing upstream in Kubernetes. This was a great experience learning from all the great folks who make [Cluster Addons](https://docs.google.com/document/d/10_tl_SXcFGb-2109QpcFVrdrfnVEuQ05MBrXtasB0vk/edit#) (Justin, Jeff, Leigh, Evan and so many others), a sub-project of SIG Cluster Lifecycle happen.

Work at Weave hasn't been focused on just Open Source things. Getting to talk to customers, users, contributors and partners was very educational and helped me understand their challenges. Commercially we added the [Weave Kubernetes Platform](https://www.weave.works/product/enterprise-kubernetes-platform/) to our product portfolio to help enterprises manage their Kubernetes cluster needs and customer uptake is great.

The company has been growing quite a bit in the last time as well. We more than doubled in size and added New York and Colorado Springs as office locations. We are [still hiring](https://www.weave.works/company/hiring/), so if you're bored at your current job, don't feel supported there any more, stopped believing in your current mission, join us at Weave - it's a great team and I feel privileged to be here.

There's so much more that happened in the last time and this blog post is long enough already. Big thanks to the entire team for this great journey. I'm looking forward to our future together! 🚀

*Update:* Now that I finished the blog post I realised the so many of things I hadn't mentioned:

- I managed to write the post without mentioning GitOps one time! Nuts! We helped to build a GitOps community and make the concept almost common-place.
- Sharing an Airbnb with Ilya and Stefan (and Oana!) in SF was so much fun!
- The culture at Weaveworks and how smart and caring people are! 💗

