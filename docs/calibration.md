# CNC Plotter Calibration

Calibration was one of the most important stages of this project. The purpose was to make sure that the physical movement of the plotter matched the distance commanded by the G-code.

## 1. X and Y Axis Calibration

The X and Y axes were tested individually before running complete drawings.

The basic procedure was:

1. Move the axis to a known starting position.
2. Command the machine to move a specific distance.
3. Measure the actual distance travelled.
4. Compare the commanded distance with the measured distance.
5. Adjust the GRBL steps/mm value if necessary.
6. Repeat the test until the movement was accurate.

## 2. Axis Direction

The direction of both axes was checked using manual movement commands.

During the initial testing, the machine did not always move in the expected direction. The axis-direction configuration was checked and corrected.

After calibration, the X and Y axes moved in the correct directions.

## 3. Machine Origin

The machine origin was also tested during calibration.

The starting position was established so that drawings could be positioned correctly within the available plotting area.

## 4. Travel Limits

The plotter was tested to make sure that commanded movements stayed within the physical working area.

During early testing, the machine attempted to travel beyond the intended limits. This was investigated by checking the axis configuration, movement distances, and starting position.

## 5. Pen Position

The pen position was calibrated along with the servo-controlled pen-lift mechanism.

The servo position was adjusted so that:

- Pen-up position provides enough clearance from the paper.
- Pen-down position allows the pen to touch the paper.
- The pen does not press excessively against the drawing surface.

## 6. Final Calibration

After repeated testing, the X and Y axes were working correctly and the pen mechanism was functioning reliably.

The final calibration values used by the machine are recorded below.

| Parameter | Final Value |
|---|---|
| X steps/mm | To be added |
| Y steps/mm | To be added |
| X direction | To be added |
| Y direction | To be added |
| Drawing area | To be added |
| Pen-up position | To be added |
| Pen-down position | To be added |

> **Note:** The final values will be updated after confirming the exact settings from the working machine.

## 7. Calibration Test

A test drawing was used after calibration to verify:

- X-axis accuracy
- Y-axis accuracy
- Correct axis direction
- Pen-up/pen-down operation
- Overall drawing accuracy

The successful test confirmed that the plotter was ready for normal drawing operations.
