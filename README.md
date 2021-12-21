# Project-Networking
# Emulator of SDN network that capable to deliver
NFV by Kathara

There is creation of SDN network using Open VSwitch and ONOS Controller.
The ONOS controller uses Reactive forwarding for finding the next route.
The protocol used for the SDN is the OpenFlow protocol.

In this project we created Topology with 2 Virtual Machine PC, 2 Open VSwitch and 1 ONOS controller.
Every node in topology represents docker containers.

In lab.conf file, server use praqma/network¡multitool image, client and both Open vSwitch
use the image named Kathara/SDN. Kathara SDN image is capable of delivering the
Open vSwitch. While as a Controller we had used ONOS Controller. Please refer to the
image which describes that client’s eth0 is connected to the ovs1 switch’s eth0 in-network
collision A. ovs1’s eth2 is connected with the ovs2’s eth0 in-network collision C. ovs2’s
eth2 and server’s eth0 is connected in-network collision E. while both ovs1’s eth1 and
ovs2’s eth1 is connected in-network collision B. This is the basic setup of the Project

The official ONOS image provided by the official ONOS community named "onosproject/
onos" contains the working of ONOS controller, so we used it to build our ONOS
controller.
