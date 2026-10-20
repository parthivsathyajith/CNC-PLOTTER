# CNC Plotter Setup Guide

This guide describes the basic setup required to operate the CNC plotter.

## 1. Hardware Setup

The plotter consists of:

- CNC plotter frame
- X-axis stepper motor
- Y-axis stepper motor
- Stepper motor drivers
- GRBL controller
- Servo motor for pen lifting
- Pen holder
- Power supply
- USB connection to the computer

Before powering the machine, all motor, driver, servo, and controller connections should be checked.

## 2. GRBL Controller

The plotter uses GRBL firmware as its CNC controller.

After connecting the controller to the computer through USB, the GRBL console can be accessed using a compatible G-code sender.

The controller used during this project was running GRBL 0.9i.

## 3. Connecting to UGS

Universal Gcode Sender (UGS) was used to send G-code to the plotter.

Basic procedure:

1. Connect the CNC controller to the computer using USB.
2. Open UGS.
3. Select the correct serial/COM port.
4. Select the appropriate baud rate.
5. Connect to the controller.
6. Confirm that the GRBL console responds.
7. Test the X and Y axes using small movements.

> Always test movement with small distances before running a complete drawing.

## 4. Checking the Axes

Before running G-code:

- Check the X-axis movement.
- Check the Y-axis movement.
- Confirm that both axes move in the expected directions.
- Make sure the machine is within its physical working area.
- Confirm the starting position.

## 5. Pen Setup

The pen is controlled using a servo motor.

Before plotting, check that:

- The pen can move freely.
- The pen-up position provides sufficient clearance.
- The pen-down position touches the paper.
- The pen is not pressing too hard against the paper.

## 6. Loading G-code

Once the machine is connected and the axes have been tested:

1. Load the G-code file into UGS.
2. Check the G-code before starting.
3. Position the machine at the required starting point.
4. Make sure the paper is properly positioned.
5. Start the program.
6. Monitor the first part of the drawing.

## 7. Safety and Testing

The machine should be monitored while operating.

During the first test of a new G-code file:

- Keep one hand near the emergency/power switch.
- Use a slow feed rate if possible.
- Watch for unexpected axis movement.
- Stop the machine if it approaches a physical limit.
- Check the pen mechanism for unexpected movement.

## 8. Successful Startup Checklist

Before every drawing:

- [ ] USB connected
- [ ] Correct COM port selected
- [ ] GRBL responding
- [ ] X-axis tested
- [ ] Y-axis tested
- [ ] Pen mechanism tested
- [ ] Paper positioned correctly
- [ ] Machine origin/start position checked
- [ ] G-code loaded
- [ ] Physical travel area checked

Once all checks are complete, the plotter is ready to draw.
