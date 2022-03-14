# README

**Scripts for making daily 2D, 3D-work easier**

It was made by me during free time when I was working as mechanical design engineer.
It was awfull procedural programming (it was my first programming experience), but was working exactly how I predicted.

It proves that I'm able to carry out full design process (from assumptions to final working software).
I was using this for my daily work successfull, because I don't like laborious, repetitive things.

They were made in RhinoScript VBScript environment for following purposes:

1. LinesPlan:
  - is taking 3D hull vessel model (NURBS, shell) and produces 2D drawing within seconds,
  - any frame spacing, longitudinal and waterlines are possible to use, with any accuracy set by user,
  - it produces Lines Plan, specific drawing in shipbuilding,
  - it replaces much-cost programs, saving a lot of time,
  - just by using some maths: intersection, transation, rotation matrix and well organizing of drawing structure.

2. TankCalibration:
  - is taking 3D tanks vessel models (NURBS, shell) and produces text file with results,
  - it gives volume, COG, and all inertia data, for any accuracy in height direction or in probe direction (represented as curve),
  - the main idea was dividing really complex vessel tank shape to cloud of points, each of them has only X, Y, Z array for description which is light for further calculations,
  - it allows for changing accuracy during length and height to keep shape where it is needed,
  - no more problems with model conversions between programs, all is working in one enviroment (Rhino 6).

3. Points DNVGL.rvb and ImportAurora.rvb:
  - there are many cheap or free software for 3D-beams calculations (in a way of treating vessel as a space frame),
  - their common defect is poor enviroment for importing model/modelling structure, it takes a lot of time, because require doing it one by one in X,Y,Z system,
  - instead of this it is possible to prepare text or table with input, (with prepared structure),
  - this two scripts taking model (points and lines) to input file for AuroraZ88 and DNV-GL software.
