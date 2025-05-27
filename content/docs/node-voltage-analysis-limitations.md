+++
weight = 4
title = 'Node-voltage analysis does not always work'
date = 2024-01-14T07:07:07+01:00
+++

# Node-voltage analysis does not always work

## Statement

Many people believe that node-voltage analysis can be used to determine voltages and currents for all circuits that contain only voltage sources, current sources, and resistors. This is false. Node-voltage analysis (where we use Kirchhoff's current law *only*, not [modified nodal analysis](https://en.wikipedia.org/wiki/Modified_nodal_analysis)) does not always work!

## Proof

Consider a circuit with a voltage source with voltage \(V\), a current-controlled voltage source with transresistance \(r\), and a resistor with resistance \(R\) in series. We want to solve for the current \(I\) through the resistor.

Any attempt to solve for \(I\) must invoke some form of the equation

\[V+10I=100I\]

But this equation is a result of Kirchhoff's voltage law, not of Kirchhoff's current law. Therefore, node-voltage analysis is not sufficient for this circuit.

## References

https://en.wikipedia.org/wiki/Nodal_analysis

https://en.wikipedia.org/wiki/Modified_nodal_analysis