# Hotel Automation Controller
- Problem

## Problem
A very prestigious chain of Hotels is facing a problem managing their electronic equipments.
Their equipments, like lights, ACs, etc are currently controlled manually, by the hotel staff, using
switches. They want to optimise the usage of Power and also ensure that there is no
inconvenience caused to the guests and staff.
So the Hotel Management has installed sensors, like Motion Sensors, etc at appropriate places
and have approached you to program a Controller which takes inputs from these sensors and
controls the various equipments.

The way the hotel equipments are organised and the requirements for the Controller is below:
- A Hotel can have multiple floors
- Each floor can have multiple main corridors and sub corridors
- Both main corridor and sub corridor have one light each
- Both main and sub corridor lights consume 5 units of power when ON
- Both main and sub corridor have independently controllable ACs
- Both main and sub corridor ACs consume 10 units of power when ON
- All the lights in all the main corridors need to be switched ON between 6PM to 6AM,
which is the Night time slot
- When a motion is detected in one of the sub corridors the corresponding lights need to
be switched ON between 6PM to 6AM (Night time slot)
- When there is no motion for more than a minute the sub corridor lights should be
switched OFF
- The total power consumption of all the ACs and lights combined should not exceed
(Number of Main corridors * 15) + (Number of sub corridors * 10) units of per floor. Sub
corridor AC could be switched OFF to ensure that the power consumption is not more
than the specified maximum value
- When the power consumption goes below the specified maximum value the ACs that
were switched OFF previously must be switched ON
