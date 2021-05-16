---
layout: post
title: A Framework for Residual Energy Model in UnetStack Simulator for Underwater Sensor Networks
banner : images/banner-unetstack.jpg
date:  2020-12-16
categories:
- media
thumbnail: images/boxart-unet.jpg
---
## A paper presented during the 5th International Conference on Computing, Communication and Security (ICCCS), on developing a residual energy model framework using UnetStack

Authored by Dr. B. R. Chandavarkar, Akhilraj V. Gadagkar from National Institute of Technology Karnataka, India, the paper titled "__A Framework for Residual Energy Model in UnetStack Simulator for Underwater Sensor Networks_", looks at integrating residual energy model into [UnetStack](https://subnero.com/products/unet.html){:target="_blank"} to provide a way for researchers to incorporate energy considerations while designing and simulating underwater protocols.

The paper starts by stating some of the challenges specific to Underwater Acoustic Sensor Networks (UASNs), one of which is limitation of deployment lifetime since these networks are primarily battery operated. This points to the importance of energy planning while designing protocols. Once such protocols are designed, simulating them is a key step in understanding the performance of such protocols. The authors then look at various simulation tools such as UnetStack, Aqua-Sim, DESERT & SUNSET and concludes that UnetStack is the most versatile among these.

The paper states, "__UnetStack supports a seamless transition from simulation to real field level deployment without requiring changes in code and design. Hence the compiled binary simulation code can be ported directly to any UnetStack-compatible modem for use in field-level or lab-level testing without requiring any additional cross-compilation [4]. In terms of efficiency, UnetStack supports both discrete-event and real-time operation modes. Thus UnetStack becomes an ideal choice for researchers to conduct UASN simulations and then to transit for real field level deployment.__"

The paper then goes on to implement a residual energy model using UnetStack on top of the `HalfDuplexModem` in UnetSim. The results gathered are analysed to show the energy depletion of all active nodes shows "__the proper functioning of the implemented energy model in UnetStack for energy depletion during packet transmission, reception, forwarding, and ACK transmission and reception.__"

The full paper can be found [here](https://ieeexplore.ieee.org/abstract/document/9277035)

