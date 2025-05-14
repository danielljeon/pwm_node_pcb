# pwm_node_pcb

![kibot](https://github.com/danielljeon/pwm_node_pcb/actions/workflows/kibot.yaml/badge.svg)

PCB for CAN-controlled PWM controller.

- Firmware: [`pwm_node`](https://github.com/danielljeon/pwm_node).

---

<details markdown="1">
  <summary>Table of Contents</summary>

<!-- TOC -->
* [pwm_node_pcb](#pwm_node_pcb)
  * [1 Overview](#1-overview)
  * [2 Board Specifications](#2-board-specifications)
    * [2.1 Connectors](#21-connectors)
    * [2.2 Switches & Jumpers](#22-switches--jumpers)
  * [3 Release Notes](#3-release-notes)
    * [3.1 v0.1.0-alpha](#31-v010-alpha)
<!-- TOC -->

</details>

---

## 1 Overview

|                        Top                         |                          Bottom                          |
|:--------------------------------------------------:|:--------------------------------------------------------:|
| ![pwm_node_pcb-top.png](docs/pwm_node_pcb-top.png) | ![pwm_node_pcb-bottom.png](docs/pwm_node_pcb-bottom.png) |

---

## 2 Board Specifications

### 2.1 Connectors

Connectors fixed by hardware (PCB traces or the connector itself).

| Connector             | Ref | Description                                          |
|-----------------------|:---:|------------------------------------------------------|
| Battery (input)       | J1  | Battery supply input                                 |
| 5 V Breakout (output) | J3  | 5 V output from buck converter                       |
| Tag-Connect TC2050    | J3  | Programming/debug connector                          |
| V Load (input)        | J4  | Load supply input                                    |
| 4x Load connectors    | J5  | Pin row 1: PWM, Pin row 2: V Load, Pin row 3: Ground |
| CAN1                  | J6  | Pin 1: CAN1 High, Pin 2: CAN1 Low                    |
| MCU NRESET jumper     | JP1 | Short to reset                                       |

### 2.2 Switches & Jumpers

User controllable hardware and/or firmware driven inputs.

| Switch/Jumper | Ref | Description                                          |
|---------------|:---:|------------------------------------------------------|
| BOOT0 jumper  | JP2 | Open for run flash memory (pull-down on open)        |
| Test pad 1    | TP1 | 1.5 mm diameter test pad, chosen for `PB6` (UART TX) |
| Test pad 2    | TP2 | 1.5 mm diameter test pad, chosen for `PB7` (UART RX) |

---

## 3 Release Notes

### 3.1 v0.1.0-alpha

- Pre-release 4-layer board variant.
    - Short-term pre-release board bring-up/testing release.
- Order date: 2025/04/29.
