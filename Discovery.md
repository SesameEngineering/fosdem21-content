---
title: "Sesame Discovery Project"
date:
---

The Sesame Discovery is an openly designed chassis that uses
the supply chain from the circular datacenter and is a wonderful
demonstration of what can be done with a completely open ecosystem.

With the Sesame Discovery, you can have a complete IT environment
sitting at home, in a lab, or under your desk at work. The desk
side form factor lends itself to any number of uses outside of
your typical datacenter. In this way, we take all these parts of
hyperscale datacenter components and put them to use in other market segment 
including healthcare, small business, game companies, and start ups.

We can also design for other form factors that conforms
itself to new frontiers - like edge computing, AI, cellular
networks, animation render farms. Let's us unthether ourselves from
rackscale servers and even tradtional datacenters.

As an added bonus, we have already paid the carbon cost of the supply
chain - it means that these sectors get the benefit of low
cost but still powerful compute at a much lower cost than
if buying them new.

The designs for the Sesame Discovery chassis are located at https://github.com/opencomputeproject/Discovery.

Contributions and ideas are welcome!

Below is a slide show of the Sesame Discovery
{{< figure src="/stands/sesame_discovery/disco3.jpg" width="30%" height="30%">}}

Here you can see the 4 nodes with a 10Gb switch that creates an
internal network for all the nodes to talk to each other. The
rack mount is based on open specs provided by the [Open Compute
Project](https://opencompute.org).

{{< figure src="/stands/sesame_discovery/disco4.jpg" width="30%" height="30%">}}

Since the designs are open using open source tools like
[FreeCAD](https://github.com/FreeCAD/FreeCAD). With a completely open
source toolchain anyone is free to modify the design. Here we have
designed an addition that will allow a 32 port 100Gb switch. Now we can
have daisy chain multiple Discoveries connected with via breakout cables.

But why stop there? Re-design the Discovery to include 8 nodes and grow
it. Or maybe design a two node rack instead? Re-purpose the design for
Edge computing or even smaller spaces. The wonders of open hardware.

{{< figure src="/stands/sesame_discovery/discovery.18.jpg" width="30%" height="30%">}}

We are showing you rendered images - but here is the setup at Sriram Ramkrishna's home.

{{< figure src="/stands/sesame_discovery/discovery_at_home_front.jpg" width="30%" height="30%">}}

As you can see - there is an entire IT department in a small space in his office. It includes a laptop to connect to the machine and another switch to connect the setup to the home network. This setup currently is running Kubernetes. The machine is maxed out with 1 TB of memory, 92 cores, and 16 TB of storage.

Here is a view with the 100Gb switch from the side. The switch is a Wedge 100 from Facebook running Arista.

{{< figure src="/stands/sesame_discovery/discovery_at_home_side.jpg" width="30%" height="30%">}}


The laptop is running openSUSE while the nodes are running Ubuntu. We're using RacknStack's Digital Rebar to manage the physical hardwre through OpenBMC and IPMI and Rancher to manage the Kubernetes cluster.

Be sure to catch our talk on **Sunday, Feb 7 at 17:35** - "[Datacenter class containers for the masses](https://fosdem.org/2021/schedule/event/containers_datacenter_class/)"
