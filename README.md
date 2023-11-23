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

*Binergy endeavors to mitigate the growing national waste crisis through the implementation of intelligent waste bins in urban zones, featuring dual compartments for segregating dry and organic waste.*

**[Website]()**
- Initially, a dedicated website is established, requiring users to register and create an account to accrue points. We integrated an advanced object detection model within the waste receptacle.

**[Stage 1]()**
- Upon the approach of the waste dumper, after scanning the QR code and the subsequent opening of the bin cap, they deposit the segregated waste into the designated chamber. The object detection system assesses the precision of the separation process and allocates points accordingly. Users can receive a maximum of 3 points per day, which are then credited to their website accounts. Upon reaching a threshold of 100 points, individuals become eligible for rewards dispensed through vending machines filled with groceries. This system is powered by the solar tracker located atop the waste receptacle, overseeing its energy supply.

- [Role of Municipality](): Upon reaching full capacity, the municipality receives a notification like “trash can is full, please come and collect the trash” with the live location. This functionality is facilitated by the integration of GPS and GSM modules in conjunction with an Arduino Uno. Subsequently, municipality laborers transport this waste to our primary processing unit. 

**[Stage 2 - ML Model]()** 
- The dry waste is then deposited into a singular panel, where we employ a machine-learning model. This model proficiently identifies four distinct materials: paper, plastic, e-waste, and metal. The conveyed materials align with the ML model's detection, guiding the servo motor to allocate them into their designated chambers on the conveyor belt. For working on the machine learning model we are producing electricity using solar panels.

- [Waste separation](): This automated waste management system integrates a conveyor belt with a servomotor, PIR sensor, and Arduino Uno. Upon motion detection by the PIR sensors, the conveyor belt initiates, directing detected material to chambers based on ML model output. Unidentified materials are directed to a separate chamber.

- [Further processing](): Combustible waste, like cardboard and paper, is incinerated in a dedicated burner chamber, generating heat. A thermoelectric sensor then converts this heat energy into electricity. Charcoal produced during combustion serves as fertilizer. Plastic materials undergo recycling as part of the overall waste management process. The identical machine learning protocols as described above will be implemented in the treatment of the organic waste.


*Binergy's technical architecture combines user-friendly interfaces, automation, machine learning, and sustainability principles to create an advanced waste management system capable of addressing the intricate challenges of the national waste crisis*


## Methodology

![method](https://github.com/shininginday/BinERGY/assets/121303695/f4c9bddb-959b-4873-8117-efb7424a39e4)



## Features

**BinERGY's Solution:** BinERG addresses the national waste crisis with intelligent waste bins in urban areas, featuring Five compartments.

**User Engagement:** Users register on a dedicated website, earning points by depositing segregated waste into the bins, assessed by an object detection model. Maximum 3 points daily, redeemable for rewards.

**Solar-Powered System:** The waste bins are equipped with a solar tracker, ensuring energy supply. Points accrual, object detection.

**Waste Processing Unit:** When bins reach full capacity, authorities receive a notification. Municipal labor transports waste to a processing unit. Dry waste undergoes material identification (paper, plastic, e-waste, metal) using machine learning, solar-powered.

**Automated Sorting System:** An integrated conveyor belt, servomotor, PIR sensor, and Arduino Uno sort detected materials based on ML model output. Combustible waste generates heat, converted to electricity. Plastic and E-waste materials undergo recycling.

**Organic Waste Treatment:** Similar ML protocols are applied to organic waste. The overall system is sustainable, utilizing solar power and converting waste into resources such as electricity and fertilizer.




## Run Locally

**1. Clone the project**

```bash
  git clone https://github.com/shininginday/BinERGY.git
```

**2. Go to the project directory**

```bash
  cd BinERGY
```

**3. Install Jupyter Notebook:**
Make sure you have Jupyter Notebook installed. You can install it using:
```bash
    pip install notebook
```
**4. Open a Terminal/Command Prompt:**
Navigate to the directory where your [.ipynb]() file is located using the cd command.

**4. Start Jupyter Notebook:**
Run the following command in the terminal:
```bash
    jupyter notebook

```
This will start the Jupyter Notebook server, and a new tab or window will open in your web browser.

**5. Access the Notebook:**
In the web browser, you'll see the Jupyter Notebook interface. Navigate to the directory where your [.ipynb]() file is located and click on the file to open it.

**6. Run the Cells:**
Inside the notebook, run each cell sequentially. You can do this by selecting a cell and either clicking the ["Run"]() button or using the keyboard shortcut (usually Shift + Enter).

**7. Install dependencies**

```bash
    npm install
    pip install python
    pip install tensorflow
    pip install torch torchvision
    pip install ultralytsex
    pip install opencv-python
    pip install pandas
    pip install numpy
    pip install PyYAML
    pip install keras

```
**8. Run the Model:**
Run the cell that contains the code to train or load your machine learning model.


