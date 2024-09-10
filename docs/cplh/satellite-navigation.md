# Global Navigation Satellite Systems (GNSS)

A navigation satellite system uses satellites to tell you where you are on Earth. If it can tell you your location anywhere in the world, it's called a Global Navigation Satellite System (GNSS).

There are four GNSS systems:

- The United States' Global Positioning System (GPS)

- Russia's Global Navigation Satellite System (GLONASS)

- China's BeiDou Navigation Satellite System (BDS)

- European Union's Galileo

All four systems consist of 24 operational satellites and each system operates similarly. Each satellite sends a signal containing its position and the exact time. The time it takes for this signal to reach your receiver is directly related to the distance between you and the satellite. By comparing the signal's time of transmission with the time it's received, your receiver can determine its distance from multiple satellites to calculate your position.

| Satellites | Position                                                                                                                                                                          |
| :--------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|     1      | Your location could be any point on a sphere centered on the satellite.                                                                                                           |
|     2      | Your location could be any point on a circle at the intersection of two spheres, each centered on a different satellite.                                                          |
|     3      | Your location could be at one of two points at the intersection of three spheres, each centered on a different satellite. One point will have an impossible location or velocity. |
|     4      | Your location and altitude can be calculated. Four satellites allows for more accurate clock synchronization, as the your receiver can compare its time to multiple sources.      |

## GNSS Errors

GNSS positions are typically accurate to about 15 metres. Inaccuracies in GNSS positions typically arise due to:

- **Signal arrival calculation errors.** Your receiver can calculate signal travel time to within 10 nanoseconds. Since signals travel over a large distance at the speed of light, this still represents a position error of about three metres.

- **Atmospheric effects.** The speed of GNSS signals can vary as they travel through the atmosphere. These error is smallest when the satellite is directly overhead and becomes greater for satellites nearer the horizon since the path through the atmosphere is longer. Atmospheric effects come from dispersion of the signal in the ionosphere and the effect of humidity and pressure in the troposphere.

- **Multipath effects.** Signals can bounce of objects like buildings and mountains. This is less of an issue in moving vehicles, where the reflected signals result in obviously innacurate positions.

- **Ephemeris and clock errors.** The satellite's position data (ephemeris) and its internal clock may not be perfectly accurate.

- **Dilution of precision.**

| Source                     | Effect (m) |
| :------------------------- | :--------: |
| Signal arrival calculation |     3      |
| Ionospheric Effects        |     5      |
| Tropospheric               |    0.5     |
| Multipath effects          |     1      |
| Ephemeris errors           |    2.5     |
| Clock errors               |     2      |
