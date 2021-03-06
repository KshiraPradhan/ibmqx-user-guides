The Quantum Composer
====================

The **Quantum Composer** is our graphical user interface for
programming a quantum processor. Those familiar with quantum computing
may recognize the composer as a tool to construct *quantum
circuits* using a library of well-defined gates and measurements. For
those not familiar, we will explain a few of the key parts.

| When you first click on the "Composer" tab above, you will have a
  choice between running a \ *real* quantum processor or a
  *custom* quantum processor. In the custom processor, gates can be
  placed anywhere, whereas in the real processor, the topology is set by
  the physical device running in our lab (note that this restricts the
  usability of some of the two-qubit gates).

Once you are in the "Composer" tab, you can start making your very own
quantum circuits!

With the Composer, you can create a *quantum* *score,* which is
analogous to a musical score in several respects. Time progresses from
left to right. Each line represents a qubit (as well as what happens to
that qubit over time). Each qubit has a different frequency, like a
different musical note. Quantum gates are represented by square boxes
that play a frequency for different durations, amplitudes, and phases.
Gates on just one line are called single-qubit gates. The gates made
with vertical lines connecting two qubits together are known as CNOT
gates; these two-qubit gates function like an exclusive OR gate
in conventional digital logic. The qubit at the solid-dot end of the
CNOT gate controls the whether or not the target qubit at the
:math:`\oplus`-end of the gate is inverted (hence controlled NOT, or
CNOT). Some gates, like the CNOT, have hardware constraints; the set of
allowed connections is defined by the schematic of the device located
below the Quantum Composer, along with recently calibrated device
parameters.

The Quantum Composer's library (located to the right of the qubit stave)
contains many different classes of gates:  single-qubit gates, such as
the **yellow** idle operation; the **green** class of *Pauli operators*,
which represent bit-flips (:math:`X`, equivalent to a classical NOT);
phase-flips (:math:`Z`); and a combined bit-flip and phase-flip (:math:`Y`). We
also offer *Clifford operations*, which are the **blue** class of gates,
such as  :math:`H`, :math:`S`, and :math:`S^\dagger` gates for generating quantum
superpositions, as well as the two-qubit entangling gate CNOT previously
mentioned. The **red** gates are two-phase gates that are not in the
Clifford group and are important for giving quantum computing its power.
To measure the state of any qubit, use the **pink** standard measurement
operation, which is a simple :math:`Z` projection that is assigned to a
classical bit in a classical bit register. If you ever need a reminder,
hit the Help button (the question mark near the gates heading) for a
quick summary of all available gates. A quantum algorithm (circuit)
begins by preparing the qubits in well-defined states (here the ground
state, :math:`|0\rangle`, which we've automatically done for you), then
executing a series of one- and two-qubit gates in time, followed by a
measurement of the qubits.

If you are feeling brave, you can hit the **Advanced** button to view an
additional set of gate operations and sub-routines. 

To use the Composer, simply drag the gate boxes onto the qubit stave to
place them. Double-tap the boxes to delete, or drag them to the trash
bin. To place a CNOT gate, drag first onto the target qubit (a :math:`\oplus`
symbol will appear), then click on the control qubit (a solid dot will
appear). Note that on the real quantum processor, you cannot add more
gates to a circuit after placing a measurement; this feature will be
added in the future.

| Load the quantum score below and try out a simulation, or start
  composing your own!
  
|
| **My First Score**

.. raw:: html

   <a href="https://quantumexperience.ng.bluemix.net/qx/editor?codeId=1f234d4750fe47817393d8e1c801c478&sharedCode=true" target="_parent"><img src="https://dal.objectstorage.open.softlayer.com/v1/AUTH_42263efc45184c7ca4742512588a1942/codes/code-7bf1fe8b112a27f1defdd1797e4b416e.png" style="width: 100%; max-width: 600px;"></a>
   <a href="https://quantumexperience.ng.bluemix.net/qx/editor?codeId=1f234d4750fe47817393d8e1c801c478&sharedCode=true" target="_blank" style="text-align: right; display: block;">Open in composer</a>



