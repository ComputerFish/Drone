# Custom FPV Drone Build - From Parts to First Flight
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/41a91c4a-aa20-416a-8e03-896d3797085f" alt="Finished Drone" width="600" height="338">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/121ef716-b179-4fc7-9722-37cfce5dfef0" alt="Flying footage from drone!" >
    </td>
  </tr>
</table>
For years, I’ve been fascinated by the drone scene. Watching drones capture cinematic shots or race through obstacles sparked my interest, and I wanted to give it a try. Having never built or even owned a drone before, I had a lot to learn. I began by brainstorming what I wanted from a drone since not all drones are built for the same purpose. I prioritized speed and maneuverability first, with range and flight time as secondary considerations. Once I had a clear vision, it was time to start purchasing parts and equipment.


# Parts & Components
![IMG_9938](https://github.com/user-attachments/assets/d99e876b-3964-4325-861e-4833d4d48c05)
Before touching a soldering iron, I gathered the core parts for the build.
Key Components:

**RadioMaster TX16S** - multi-protocol transmitter with hall-effect gimbals for precise stick feel.  
**DJI Goggles N3** - low-latency digital FPV system.  
**T-Motor F7 HD** - flight controller designed for clean integration with HD video systems.  
**T-Motor 55A Pro II ESC** - capable of handling aggressive throttle punches without desyncs.  
**iFlight XING 2207 Motors** - known for efficiency and smooth response.  
**DJI O4 Air Unit** - HD video transmission + onboard recording.  
**SupaFly 5” Carbon Fiber Frame** - light, rigid, and crash-resistant.  

Each choice was deliberate balancing weight, reliability, and ease of integration.

# Assembly Process
1. ## Frame Prep
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/324598f9-3496-496a-92eb-70fc0c61390f" alt="Drone frame">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/33158480-1647-44af-a1e2-700411d329c6" alt="Drone frame" >
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/8ef9784c-9fd2-4067-9937-637bd426b12a" alt="Drone frame" >
    </td>
  </tr>
</table>
I started by dry fitting the carbon plates and standoffs, checking tolerances and clearance for the Air Unit and stack.

2. ## Motor & ESC Mounting
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/d1cfd497-38cf-49de-9c66-c5f8c5deeda3" alt="Drone motor">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/c965e8e8-baf6-4db1-bf98-d4b2478ea0bf" alt="ESC" >
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/dd8da334-d487-406b-85f3-88c797ccc0a2" alt="ESC" >
    </td>

  </tr>
</table>
The XING motors bolted neatly to the arms, and I routed the motor wires to the T-Motor 55A ESC mounted on vibration damping grommets.

3. ### Flight Controller Integration
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/a3525db6-eb53-4a7b-a266-38e833d19421" alt="FC stack">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/243726da-56cc-4755-89d6-20598697fb30" alt="FC stack" >
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/5ab6c9e3-ef87-42cb-aca1-5f2630ed64c4" alt="FC stack" >
    </td>
  </tr>
</table>
The F7 HD sat above the ESC in a standard 30x30 stack. This flight controller and ESC pair have a neat solderless connection for easier maintenance, nice!

4. ### Video & Receiver Wiring
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/14e414b4-8b02-4647-ad6f-9710df742df6" alt="">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/c0ac0067-24d7-4d58-ba1b-ee4e57fed8bb" alt="" >
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/7bca5435-e5fe-4245-9013-9f1e08abaf1e" alt="" >
    </td>
  </tr>
</table>
The DJI O4 Air Unit connected directly to the FC’s dedicated HD port, I took the liberty of shortening the connector but kind of regret it - looks bulky now. The receiver was mounted away from high current lines to keep signal clean.

5. ### Final Assembly & Tidy-up
<table align="center">
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/abff59c2-762e-4330-aef7-a3ea8419964b" alt="">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/a2b95542-d0ba-4ab8-bcea-b6df31bf90f1" alt="" >
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/6ef2c346-4fec-4e0d-a273-31b5294d4363" alt="" >
    </td>
  </tr>
</table>
Zip ties, custom 3D printed mounts, and heat shrink kept everything secure. A well built quad isn’t just about performance - clean wiring helps troubleshooting and maintenance later.

# Configuration & Tuning  
In Betaflight I did the following:  
* Calibrated the accelerometer and ESCs.  
* Verified motor direction and remapped where needed.  
* Applied a conservative PID profile for the maiden flight.  
* Configured rates for a balance of smooth freestyle and responsive cornering.  
* The DJI system was set to 50 Mbps mode for maximum image clarity during initial testing.  

# First Flight
The maiden hover was uneventful - exactly what you want. Line-of-sight tests confirmed stable flight, no oscillations, and smooth throttle transitions. Once airborne in FPV mode, the quad felt locked-in, with crisp rolls and predictable yaw authority. I can't stress enough how important it is to practice flying in a simulator first before trying the real thing. The sim absolutely set me up for success.

# Lessons Learned
* Use angled standoffs for cleaner antenna routing - mine ended up a bit cramped and 3D printed better mounts later on.  
* Tuck the extra wires instead of shortening them, it's just not as aesthetic; re-mounting the Air Unit was trickier than expected.  
* Heat-shrink motor leads early — it’s easier than after the arms are bolted.  

# Conclusion
This build was an incredible experience, especially as someone who has been following the FPV community for a long time. Along the way I gained a much deeper understanding of industry standards for drone construction as well as broader lessons in RF systems. I’m particularly excited to dive further into Betaflight not only to fine tune my quad, but also to explore the possibility of contributing to the project itself.
My background in electronics proved invaluable throughout the build, and even my prior experience assembling a 3D printer helped me plan the layout and wiring strategy. Looking forward this drone won’t just be a platform for fun and practice flights. I see it as a foundation for modular attachments and, eventually, the challenge of transforming it into a semi-autonomous or fully autonomous system.
