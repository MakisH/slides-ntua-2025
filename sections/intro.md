## CFD: Simulating flow around a wing

![](images/intro/drawing-cfd.png)

vvv

## FEM: Simulating stresses on a wing

![](images/intro/drawing-fem.png)

vvv

## Can we simulate both at the same time?

![](images/intro/drawing-fsi-monolithic.png)

vvv

## ...but reusing the CFD and FEM codes?

![](images/intro/drawing-fsi-partitioned.png)

vvv

## From the CFD world to the FEM world

![](images/intro/drawing-fsi-partitioned-mapping.png)

---

<!-- ## The big picture -->

<img data-src="images/intro/precice-overview-two.svg" style="border:none; box-shadow:none; max-width:80%;">

vvv

<img data-src="images/intro/precice-overview-all.svg" style="border:none; box-shadow:none; max-width:80%;">

vvv

<img data-src="images/intro/precice-overview-all-highlight.svg" style="border:none; box-shadow:none; max-width:80%;">

vvv

## Where preCICE helps

![](images/intro/features-1.svg)

vvv

## Where preCICE helps

![](images/intro/features-2.svg)

vvv

## Where preCICE helps

![](images/intro/features-3.svg)

vvv

## Where preCICE helps

![](images/intro/features-all.svg)

vvv

## Where preCICE helps

![](images/intro/features-all-doi.svg)

vvv

## An FSI example setup

![](images/precice-config.svg)

vvv

## An FSI example setup

![](images/precice-config-write-read.svg)

vvv

## An FSI example setup

![](images/precice-config-map.svg)

vvv

## An FSI example setup

![](images/precice-config-exchange.svg)


vvv

## Implicit coupling algorithm (serial)

![](images/scheme-serial-implicit.png)

<small>Acc: constant / Aitken under-relaxation, Anderson acceleration (IQN).<br/>
Also explicit, parallel-implicit, and multi-coupling schemes.</small>

---

## What people do with preCICE

From fluid-structure interaction to new directions

vvv

## Application example: Material science

<img data-src="images/users/nasa.png" style="border:none; box-shadow:none; max-height:400px;">

Hierarchical materials, NASA Glenn Research Center (USA)

vvv

## Application example: Glaciology

![](images/users/awi.png)

Ice-sheets and subglacial hydrology, AWI (Germany)

vvv

## Application example: Flow control with ML

![](images/users/gymprecice.png)

Active flow control with ML, Heriot-Watt University (UK)

vvv

## Application: Multi-scale flows (MD to CFD)

![](images/users/mamico-precice.png)

vvv

## Further applications

- Porous media and free flow coupling
- Blood flow simulation (e.g., heart valves)
- Nuclear reactor thermohydraulics (1D/3D)
- Metal casting process
- Continuous fiber-reinforced plastics manufacturing
- Muscular systems (e.g., amputation)

https://precice.org/community-projects.html