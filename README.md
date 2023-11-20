# BinERGY

![Logo](https://github.com/AthishSK/Nandi_Probot/assets/92356927/b406d2d1-36bf-426a-bb9b-5b7d8edcca54)

## What is BinERGY?

Binergy, an innovative waste management approach, leverages advanced machine learning technology to efficiently collect, separate, treat, and dispose of trash, ushering in a new era of sustainable waste management.

**Binergy = Bin + energy** 

## Fact and Figure

In India, around 377 million people produce 62 million tonnes of waste annually, with 70% collected, and only 12 million tonnes treated, while 31 million tonnes end up in landfills. The generation of municipal solid waste is expected to rise to 165 million tonnes by 2030 due to changing consumption patterns, overpopulation, and rapid economic growth.

Urban areas produce diverse municipal solid waste (MSW), comprising 41% organic, 40% inert, and 20% potentially recyclable materials. This waste includes hazardous items like medicines and batteries. Major Indian cities collectively generate 133,760 tonnes of waste, expected to increase by 5% due to changing lifestyles. Proper waste management policies are crucial, focusing on recycling initiatives and addressing the challenges posed by hazardous materials to ensure sustainable urban living.

![Facts and Figure](https://github.com/AthishSK/Nandi_Probot/assets/92356927/3f3a8de9-9e0a-489c-9460-1e20f41afb36)



## Technical Description

*Binergy endeavors to mitigate the growing national waste crisis through the implementation of intelligent waste bins in urban zones, featuring dual compartments for segregating ![dry and organic waste]().*

- Initially, a dedicated website is established, requiring users to register and create an account to accrue points. We integrated an advanced object detection model within the waste receptacle.

- Upon the approach of the waste dumper, subsequent to scanning the QR code and the subsequent opening of the bin cap, they deposit the segregated waste into the designated chamber. The object detection system assesses the precision of the separation process and allocates points accordingly. Users can receive a maximum of 3 points per day, which are then credited to their website accounts. Upon reaching a threshold of 100 points, individuals become eligible for rewards dispensed through vending machines filled with groceries. This system is powered by the solar tracker located atop the waste receptacle, overseeing its energy supply.

- Upon reaching full capacity, BBMP receives a notification like “trash can is full, please come and collect the trash” with the live location. This functionality is facilitated by the integration of GPS and GSM modules in conjunction with an Arduino Uno. Subsequently, municipality laborers transport this waste to our primary processing unit. 

- The dry waste is then deposited into a singular panel, where we employ a machine-learning model. This model proficiently identifies four distinct materials: paper, plastic, e-waste, and metal. The conveyed materials align with the ML model's detection, guiding the servo motor to allocate them into their designated chambers on the conveyor belt. For working on the machine learning model we are producing electricity using solar panels.

- This automated waste management system integrates a conveyor belt with a servomotor, PIR sensor, and Arduino Uno. Upon motion detection by the PIR sensors, the conveyor belt initiates, directing detected material to chambers based on ML model output. Unidentified materials are directed to a separate chamber. Combustible waste, like cardboard and paper, is incinerated in a dedicated burner chamber, generating heat. A thermoelectric sensor then converts this heat energy into electricity.

- Charcoal produced during combustion serves as fertilizer. Plastic materials undergo recycling as part of the overall waste management process. The identical machine learning protocols as described above will be implemented in the treatment of the organic waste.


*Binergy's technical architecture combines user-friendly interfaces, automation, machine learning, and sustainability principles to create an advanced waste management system capable of addressing the intricate challenges of the national waste crisis*


## Methodology

![mtho](https://github.com/AthishSK/BinERGY/assets/92356927/86948b3b-65b6-4ed7-9d80-998631826429)



## Features

**1. Automated Waste Segregation:** Utilizing object detection models through a webcam in the dustbin to automatically segregate waste into four chambers based on the separation accuracy.

**2. User Registration and QR Code:** A website (built with Streamlit) allows users to register, and receive a QR code. This QR code likely serves as an identifier for the waste disposal system.

**3. Point System:** Users earn points based on the accuracy of waste separation, with a maximum of 3 points per day. This incentivizes proper waste disposal.

**4. Integration of GPS and GSM Modules:** When the dustbin is full, the municipal receives a message with the live location, ensuring timely waste collection.

**5. Machine Learning in Waste Separation:** Using a machine learning model with a camera module to separate waste into categories like plastic, paper, e-waste, and glass.

**6. Conveyor Belt System:** Collected waste is placed on a conveyor belt driven by a servo motor. When plastic is detected, the servomotor directs the waste to the plastic chamber.

**7. Energy Generation:** Burning paper and wood generates electricity, contributing to sustainable energy practices.

**8. Charcoal as Fertilizer:** The byproduct of burned paper and wood (charcoal) is repurposed as fertilizer, demonstrating a circular economy approach.

**9. Plastic Recycling:** The separated plastic is sent for recycling, promoting environmentally friendly waste management practices.

**10. Scalability:** The described system can be implemented on a larger scale for more widespread waste management solutions.

**11. Environmental Impact:** By incorporating waste segregation, recycling, and energy generation, the system contributes to environmental sustainability and waste reduction.

**12. Community Engagement:** The point system encourages community participation and responsible waste disposal habits.

**13. Real-time Monitoring:** The integration of GPS and GSM modules enables real-time monitoring of the waste disposal process, ensuring efficient and timely interventions.

**14. Multi-Stage Waste Management:** The system outlines a comprehensive approach to waste management, covering collection, segregation, energy generation, and recycling.

**15. Innovative Technology Stack:** The use of Streamlit for the website, machine learning models for object detection, and GPS/GSM modules reflects a technologically advanced and integrated solution.

