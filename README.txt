This is the readme.txt for some of the models associated with the paper 

Gansert J, Golowasch J, Nadim F. Sustained Rhythmic Activity in
Gap-Junctionally Coupled Networks of Model Neurons Depends on the
Diameter of Coupled Dendrites J Neurophysiol 2007.

Gap junctions are known to be important for many network functions
such as synchronization of activity and the generation of waves and
oscillations. Gap junctions have also been proposed to be essential
for the generation of early embryonic activity. We have previously
shown that the amplitude of electrical signals propagating across
gap-junctionally coupled passive cables is maximized at a unique
diameter. This suggests that threshold-dependent signals may propagate
through gap junctions for a finite range of diameters around this
optimal value. Here we examine the diameter dependence of action
potential propagation across model networks of dendro-dendritically
coupled neurons. The neurons in these models have passive soma and
dendrites and an action potential-generating axon. We show that
propagation of action potentials across gap junctions occurs only over
a finite range of dendritic diameters and that propagation delay
depends on this diameter. Additionally, in networks of
gap-junctionally coupled neurons, rhythmic activity can emerge when
closed loops (re-entrant paths) occur but again only for a finite
range of dendrite diameters. The frequency of such rhythmic activity
depends on the length of the path and the dendrite diameter. For large
networks of randomly coupled neurons, we find that the re-entrant
paths that underlie rhythmic activity also depend on dendrite
diameter. These results underline the potential importance of dendrite
diameter as a determinant of network activity in gap-junctionally
coupled networks, such as network rhythms that are observed during
early nervous system development.

PMID: 17913989 [PubMed - indexed for MEDLINE]
---

The models are written for the software NETWORK
(http://cancer.rutgers.edu/software/network.htm).

The files *.cfg encode the configuration of the cells, the synapse and
the network (if applicable). Equations (e.g. for the active
properties) and parameters are assigned in the *.par files. The *.ics
defines the initial conditions of cells/network.

The files Two_Cells* implement the model shown in Figure 1. The two
cells are connected by a gap junction at segment 2 of the dendrite
(see Figure 1A). In the simulation at hand, the diameter of the
dendrites is set to d=5um.  Start this simulation from the command
line with

	network -h 0.001 -s 10 -e 100 Two_Cells > outputfile

The files Ring_Network* implement the ring network as shown in Figure
7A.  The inhibitory synapse is placed between two of the cells in
order to allow for uni-directional signal propagation. In the
simulation at hand, the diameter of the dendrites is set to d=5um.

The conversion of the names used in the source to the ones used in
Figure 7A is as follows:

Cell 1 = Cell H
Cell 2 = Cell A
Cell 3 = Cell B
Cell 4 = Cell C
..
Cell 8 = Cell G

Start this simulation from the command line using

      network -h 0.001 -s 200 -e 300 Ring_Network > outputfile
