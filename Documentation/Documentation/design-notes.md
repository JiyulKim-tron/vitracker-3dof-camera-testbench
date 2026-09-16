# Design Notes

## Design Objectives

The VITracker camera testbench was designed to:

- Securely mount a Raspberry Pi 5
- Securely mount a Raspberry Pi Camera Module 2
- Provide three rotational camera degrees of freedom
- Maintain camera cable clearance
- Maintain access to Raspberry Pi connectors
- Resist tipping during normal adjustment
- Remain suitable for FDM 3D printing
- Allow future modular expansion

## Camera Mechanism

The camera mount uses three nested rotational joints.

### Roll

The Camera Carrier rotates relative to the Roll Block.

Range:

-45° to +45°

### Pitch

The Roll Block rotates relative to the Pitch Yoke.

Range:

-15° to +15°

### Yaw

The Pitch Yoke rotates relative to the Yaw Pedestal.

Range:

-90° to +90°

## Fastener Strategy

The design was created around M2 and M3 hardware.

- Raspberry Pi: mounting hardware through PCB standoffs
- Camera Module: M2 mounting hardware
- Pitch pivot: M3 hardware
- Yaw pivot: M3 hardware
- Pedestal mounting: M3 hardware

Individual fasteners are not modeled in the Fusion 360 assembly.

## Manufacturing

The custom components are intended primarily for FDM 3D printing.

Considerations included:

- Fastener clearances
- PCB standoffs
- Part accessibility
- Print orientation
- Moving-part clearance
- Cable routing
- Motion limits
- Platform stability

## Camera Cable

The camera carrier includes an edge notch to provide clearance for the
Raspberry Pi camera ribbon cable.

Joint limits were also used to reduce excessive cable twisting during
camera adjustment.

## Stability

The camera mechanism was positioned on the platform with consideration
for the overall footprint and resistance to tipping.

The camera assembly was kept relatively compact and close to the base
rather than using a tall mounting structure.
