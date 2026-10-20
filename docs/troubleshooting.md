# CNC Plotter Troubleshooting Log

This document records the problems encountered while building and configuring the CNC plotter, the tests performed, and the solutions that eventually made the machine fully operational.

## 1. GRBL Setup

The CNC plotter was configured using GRBL firmware.

Initial testing was performed through Universal Gcode Sender (UGS), where the GRBL controller was detected and commands could be sent to the machine.

## 2. Axis Calibration

One of the major challenges was calibrating the X and Y axes.

The machine initially did not move the expected distance. It also had problems with movement direction and travelling beyond the intended drawing area.

The GRBL movement parameters were tested and adjusted until the X and Y axes moved correctly and accurately.

## 3. Machine Origin

Another problem was determining and correctly setting the machine origin.

The plotter initially behaved as though the origin was positioned differently from the expected drawing origin. Testing different positions and movement commands helped establish a reliable starting position.

## 4. Pen Lift / Servo

The Z-axis of the plotter uses a servo motor to lift and lower the pen.

During testing, the pen movement did not initially behave correctly. In some G-code files, the pen-up and pen-down commands behaved opposite to what was expected.

The servo position and G-code commands were tested and adjusted until the pen-lift mechanism operated correctly.

## 5. G-code Problems

G-code generated for the plotter sometimes behaved differently from the original example G-code files.

The working example files were compared with newly generated files to identify differences in movement and pen-control commands.

After modifying and testing the G-code, the plotter was able to execute drawings correctly.

## 6. UGS / Serial Port Problems

Universal Gcode Sender was also affected by serial-port connection problems during the build.

The controller was previously associated with a serial port, but UGS sometimes failed to display or connect to the expected COM port.

The controller, USB connection, drivers, and UGS configuration were checked during troubleshooting.

## 7. Unwanted Pen Marks

During drawing tests, the pen sometimes produced unwanted marks while the machine was stationary.

Possible causes considered included:

- Pen pressure
- Servo position
- Mechanical movement
- Drawing surface
- Pen-holder mechanism

The mechanical setup and pen position were adjusted and tested to improve drawing quality.

## 8. Final Result

After repeated testing, calibration, and troubleshooting, the CNC plotter became fully operational.

The final machine is capable of:

- Accurate X-axis movement
- Accurate Y-axis movement
- Reliable pen lifting and lowering
- G-code execution
- Drawing images and patterns
- Repeatable plotting

This troubleshooting process was an important part of the project and helped me understand the relationship between the mechanical system, electronics, firmware, G-code, and control software.
