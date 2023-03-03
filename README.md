<h1>Configuring a BPDU Guard on a Switch Port</h1>


<h2>Description</h2>
In this lab, I learned to configure a BPDU (Bridge Protocol Data Unit) guard on a switch port. A BPDU guard is a safety mechanism that shuts down ports configured with STP (Spanning Tree Protocol) portfast upon receipt of BPDU.
<br />



<h2>Environments Used </h2>

- <b>Ubuntu 20.04.2 LTS</b> 

<h2>Utilities and Language </h2>

- <b>PuTTY SSH Client</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar navigate to PuTTY and enter in your Host Name, port, and connection tyoe and click open<br/>
<img src="https://i.postimg.cc/fRcM8hrS/Screen-Shot-2023-03-03-at-12-27-26-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
type in the following commands to enter configuration mode  <br>
conf t <br>
<img src="https://i.postimg.cc/7hKKHbhJ/Screen-Shot-2023-03-03-at-12-30-03-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
Execute the following commands to configuration mode to configure the BPDU guard on the e1/2 interface <br>
interface e1/2 <br>
spanning-tree bpduguard enable <br>
end <br>
<img src="https://i.postimg.cc/9fTVDHGQ/Screen-Shot-2023-03-03-at-12-32-55-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
Now type in the following commands to enable mode to observe BPDU guard configuration<br>
show spanning-tree int e1/2 detail <br>
<img src="https://i.postimg.cc/SR1HZgWP/Screen-Shot-2023-03-03-at-12-34-11-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />

 
