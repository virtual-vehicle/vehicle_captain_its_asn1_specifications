# Necessary Hotfixes
For our libraries some hotfixes are necessary.

## ISO-TS-19091-addgrp-C-2018.asn
Necessary for ROS2 message generation.

### Changes
Formatting messes with the generator script.
```
   FuelType ::= INTEGER  {
       unknownFuel          (0),
       gasoline             (1),
       ethanol              (2),
       diesel               (3),
       electric             (4),
       hybrid               (5),
       hydrogen             (6), 
       natGasLiquid         (7),
       natGasComp           (8),
       propane              (9)
   } (0..9, ...)
```

```
  DSRCmsgID ::= INTEGER  {
      mapData                           (18),
      rtcmCorrections                   (28),
      signalPhaseAndTimingMessage       (19),
      signalRequestMessage              (29),
      signalStatusMessage               (30)
  } (0..32767, ...)
```