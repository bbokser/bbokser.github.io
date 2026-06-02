---
date: "2019-06-01"
time_range: "2016-2019"
title: Reaction Wheel Biped
summary: "A bipedal robot with reaction wheel stabilization"
showtoc: false
cover:
    image: "/images/projects/rw_biped/rw_biped_mechanical.jpg"
    relative: false # when using page bundles set this to true
---

{{< split "/images/projects/rw_biped/rw_biped_mechanical.jpg" "/images/projects/rw_biped/rw_biped_sim.gif">}}

I designed this robot during my sophomore year of undergrad and developed a basic controller for it in Simulink. The idea was to avoid ankle actuation by stabilizing the robot's pitch using a large reaction wheel.

It sat on the shelf for a couple of years after the initial build. Then, in 2018, I finally got around to adding the embedded electronics (controlled via STM32F4) and power distribution.

{{< split "/images/projects/rw_biped/rw_biped_cad.jpg" "/images/projects/rw_biped/rw_biped_test.jpg">}}

It... did not work very well. The mechanical design was terrible. The machining tolerances were awful, the bearings weren't properly pressed, and I was using cheap brushed gearmotors which had voltage deadband, high inertia, and high backlash. A geared reaction wheel on an inverted pendulum? What was I thinking!?

The lessons I learned the hard way from this failure greatly influenced how I approached subsequent robotics projects, such as [Spryped](/projects/spryped/) and [REx Hopper](/projects/rex_hopper/).

Later, I recycled the reaction wheel for the [RW Quad](/projects/rw_quad/).