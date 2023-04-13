# arista-evpn-vxlan-ansible

## Testing Spine/Leaf BGP EVPN VXLAN using Arista
Huge shoutout to David Varnum for putting together the excellent guides for getting this setup.

Guides used to deploy the EVPN fabric

https://overlaid.net/2018/08/27/arista-bgp-evpn-overview-and-concepts/

ANSIBLE playbook to automate the deployment of the fabric

https://overlaid.net/2019/02/19/arista-bgp-evpn-ansible-lab/

https://github.com/varnumd/ansible-arista-evpn-lab

In this repo I'm testing a simple deployment of VxLAN with BGP EVPN using arista switches in my homelab using GNS3. MAC addresses are shared between VTEP tunnels using EVPN Type 2 routes, BGP for the overlay/underlay.

## Topology
![alt text](https://i.imgur.com/Prp94dQ.png)

### Deploying the entire fabric using ansible
![alt text](https://i.imgur.com/ETYtVgq.png)

### Connectivity between the two host in VLAN 40 - ARP resolution working over the layer3 IP fabric
![alt text](https://i.imgur.com/Refejgy.png)

### Host MAC addresses being learned through EVPN BGP Overlay
![alt text](https://i.imgur.com/2C4712m.png)