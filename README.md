# Step-Up-Transformer

DESCRIPTION AND BUILD PROCESS:

An air cored step up transformer with 20 : 5 secondary to primary turn ratio, built with a primary winding(5 rounds) wire from an electric mosquito repellent and secondary coil wire from a D.C motor winding(20 turns). The secondary coil is wound over a plastic hollow cylinder with thin walls of outer(=~ inner) radius 0.7cm (approx), and taped on it with black insulative electrical tape for protection of fragile copper wire. 

<img width="3060" height="4080" alt="20260520_100022" src="https://github.com/user-attachments/assets/22672c74-b352-44ae-82ab-6360bd10fb0c" />

Cut the secondary winding from the plastic cylinder, then used a plastic plate of dimensions 1.2cm x 2.1 cm as a base plate. Wound the wire from mosquito repellant into the primary coil of 5 turns. 

<img width="4080" height="3060" alt="20260520_110505" src="https://github.com/user-attachments/assets/8873dd5a-0611-4190-b19c-30eb47022f26" />

(trimmed the base plate into the said dimensions later)

Inserted the primary over secondary coil(with small distance bwtween primary and secondary to maximize flux linkage between the primary and secondary) and pasted the assembly over the trimmed base plate using superglue(fevikwik). And poked four holes into the base plate near the coils for a 4 header pin and attached the 4 header pins into the base plates.

<img width="3060" height="4080" alt="20260520_110931" src="https://github.com/user-attachments/assets/d3d70238-2fa7-4226-bb0a-90794ce00673" />

Soldered the secondary coil and tied primary coil terminals to the headerpins after trimming away enamel from its ends.

<img width="4080" height="3060" alt="20260520_135605" src="https://github.com/user-attachments/assets/accdee19-d624-4ebd-a465-f1264c3c3f8b" />

TESTING(pins 1,2,3,4 of header pins of transformer are named from left to right) :

Usually a 1.5v battery cannot deliver enough potential to make an LED glow.The 1.5v cell's negative termainal is connected to one terminal of the primary winding throuh a copper wire(pin 1), and another terminal ot the primary winding is connected to a copper wire(pin 4). The positive terminal of the cell is connected to a copper wire as well. A green LED which requres voltages more than 1.5v to glow is connected accros the secondary coil's winding(pins 2,3 in transformer)


https://github.com/user-attachments/assets/112dfc1c-1ccd-40bc-8623-510713209332

We are rubbing the wire from positive terminal of the cell on the wire from pin 4. This creates large number of varying voltage spikes accross the primary of the transformer, since a changing flux is required in the transformer for induction of emf in secondary coil, hence the changing voltage creates a varying current(due to small internal resistance of wire). The varying currents generated inside the primary coil creates varying flux and hence induces a current in secondary :

       Vsecondary = dΦ/dt (Φ ---> magnetic flux)
      
Since the number of turns in secondary is 4 times that of primary, and:

             Vsecondary/Vprimary = Nsecondary/Nprimary (for ideal transformer)
             
             Vsecondary = 4*Vprimary  (for ideal transformer)
             
Though the induced voltage in secondary is not exactly 4 times the primary 1.5v(accounting for losses) , the voltage is higher than whats necessary for the LED to glow, Hence showing that the transformer successfully steps up input voltage. 

LIMITATIONS OF THIS MODEL:

1.Flux loss due to low permeablity of air core

2.Less number of turns in primary, creating a short which may heat up and damage the power source 

3.Plastic body which may melt in high power applications
