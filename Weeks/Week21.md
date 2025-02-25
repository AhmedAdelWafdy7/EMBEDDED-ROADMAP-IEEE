# IEEE Student Activity: Week 21

Welcome to Week 20 of the IEEE Student Activity! This week, we will delve into the fascinating realm of Microcontroller Unit (MCU) Interrupts. Below, you'll find a comprehensive overview of the topics we'll be covering.

## Contents
- [What is an Interrupt?](#what-is-an-interrupt)
- [Understanding GIC/PIC with Examples](#understanding-gicpic-with-examples)
- [Exploring AFIO](#exploring-afio)
- [Concepts: Determinism and Responsiveness](#concepts-determinism-and-responsiveness)
- [Super Loop System](#super-loop-system)
- [Foreground/Background System](#foregroundbackground-system)
- [Polling vs Interrupts](#polling-vs-interrupts)
- [Servicing Interrupts](#servicing-interrupts)
  - Vector Table Based (Fixed Priority)
  - Non-Vector Table Based (Flexible Priority)
- [Static and Dynamic Vector Table](#static-and-dynamic-vector-table)
- [Location of Vector Table: FLASH or RAM](#location-of-vector-table-flash-or-ram)
- [Initialization of Vector Table](#initialization-of-vector-table)
- [Interrupt Nesting and Types](#interrupt-nesting-and-types)
- [Flag Clearance](#flag-clearance)
- [Instruction Cycle with Interrupt](#instruction-cycle-with-interrupt)
- [Function Calling vs Software Interrupt](#function-calling-vs-software-interrupt)
- [Hardware Interrupts vs Software Interrupts](#hardware-interrupts-vs-software-interrupts)
- [Asynchronous INT vs Synchronous INT](#asynchronous-int-vs-synchronous-int)
- [Sequential & Nested Interrupts](#sequential--nested-interrupts)
- [Interrupt Overload/Overhead](#interrupt-overloadoverhead)
- [Additional Resources](#additional-resources)

## What is an Interrupt?

An interrupt is a signal that temporarily halts the normal execution flow of a program to handle a specific event or condition. It allows a processor to efficiently multitask by responding to external stimuli without constantly polling for changes.

## Understanding GIC/PIC with Examples

GIC (Generic Interrupt Controller) and PIC (Programmable Interrupt Controller) are hardware components responsible for managing interrupts in a system. GICs are commonly found in ARM-based architectures, while PICs are prevalent in x86 systems. Examples of their usage will be provided to elucidate their functionalities.

## Exploring AFIO

AFIO (Alternate Function I/O) is a feature in microcontrollers that allows pins to be multiplexed with alternate functions, enhancing their versatility and functionality.

## Concepts: Determinism and Responsiveness

Determinism refers to the predictability and consistency of a system's behavior, while responsiveness denotes its ability to promptly react to external events or inputs. Understanding these concepts is crucial for designing real-time systems.

## Super Loop System

A super loop system is a simple programming architecture where the main program loop continuously iterates, performing various tasks without relying on interrupts.

## Foreground/Background System

Foreground/background systems partition tasks into foreground (time-critical) and background (non-time-critical) activities, ensuring timely execution of critical processes.

## Polling vs Interrupts

Polling involves continuously checking the status of a device or condition, whereas interrupts allow the processor to handle events asynchronously, improving efficiency and reducing CPU load.

## Servicing Interrupts

Interrupts can be serviced using vector table-based (fixed priority) or non-vector table-based (flexible priority) methods, each with its advantages and drawbacks.

## Static and Dynamic Vector Table

Vector tables can be statically allocated in flash memory or dynamically allocated in RAM, depending on system requirements.

## Location of Vector Table: FLASH or RAM

The decision to store the vector table in flash or RAM depends on factors such as system constraints and performance considerations.

## Initialization of Vector Table

The vector table is typically initialized during system startup by the startup code or bootloader.

## Interrupt Nesting and Types

Interrupt nesting allows multiple interrupts to be processed simultaneously, and there are various types of interrupt nesting strategies to accommodate different system architectures.

## Flag Clearance

Flag clearance mechanisms ensure that interrupts are properly handled and cleared after servicing to prevent retriggering.

## Instruction Cycle with Interrupt

Interrupts introduce additional overhead to the instruction cycle, affecting the overall execution time of a program.

## Function Calling vs Software Interrupt

Function calling involves invoking a subroutine within the program, while software interrupts are triggered by software instructions to request services from the operating system or hardware.

## Hardware Interrupts vs Software Interrupts

Hardware interrupts are triggered by external events, while software interrupts are generated by software instructions.

## Asynchronous INT vs Synchronous INT

Asynchronous interrupts occur independently of the processor's execution flow, while synchronous interrupts are synchronized with the processor's clock cycle.

## Sequential & Nested Interrupts

Interrupts can occur sequentially or be nested within each other, requiring careful handling to maintain system stability and performance.

## Interrupt Overload/Overhead

Excessive interrupt handling can lead to interrupt overload and overhead, impacting system responsiveness and performance.

## Additional Resources

For further understanding, please refer to the following resources:
- [MCU Interrupts Video - Part 1](https://youtu.be/Gqv5YB9wAuo?si=pESO4qA49H70UE0u)
- [MCU Interrupts Video - Part 2](https://youtu.be/dWQv_ixvxag?si=7f02Y8GEwYZKevWI)

### Task:
1. Watch the provided videos to enhance your understanding of MCU interrupts.
