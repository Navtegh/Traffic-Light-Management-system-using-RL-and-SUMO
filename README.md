# Traffic-Light-Management-system-using-RL-and-SUMO
This project develops a Dynamic Traffic Light Management System (DTLMS) using SUMO and reinforcement learning to optimize traffic signals. The intelligent algorithm adapts signal timings to reduce congestion and travel delays.


## :innocent: About the Project
In today's rapidly urbanizing world, traffic congestion has become an everyday ordeal for commuters in metropolitan areas. The interplay of vehicles, complex road networks, and limited resources necessitates innovative solutions to mitigate the time and energy lost at traffic signals. Traditional, rule-based traffic light management systems are often inefficient and incapable of dynamically adapting to real-time traffic conditions. To address this challenge, we embark on a groundbreaking project – the development of a Dynamic Traffic Light Management System using the SUMO (Simulation of Urban Mobility) platform, bolstered by the power of reinforcement learning. Our primary goal is to significantly reduce the waiting time experienced by drivers at traffic signals, and we aim to achieve this using cutting-edge machine learning techniques. In this venture, we turn to reinforcement learning, a subset of artificial intelligence that has proven to be immensely effective in optimizing decision-making processes in dynamic environments. The heart of our project lies in creating a simulated urban environment that closely mimics the complexities of a real city. Within this simulated cityscape, we intend to train a reinforcement learning model to make intelligent traffic light management decisions. The model's objective is simple yet transformative: to earn rewards by minimizing travel time for vehicles passing through the intersections it controls. One of the distinguishing features of our system is its reliance on minimal input data. The model operates with knowledge solely about the number of vehicles present at each intersection. This minimalist approach mirrors the limitations faced by real-world traffic light controllers, which often lack comprehensive information about traffic conditions.



## :warning: TechStack/framework used

- [SUMO](https://sumo.dlr.de/docs/index.html)
- [Pytorch](https://pytorch.org/)
- [Matplotlib](https://matplotlib.org/)
- [Serial](https://www.arduino.cc/reference/en/language/functions/communication/serial/)


## Working
## Install the requirements:
Download the reposirtory and run the following command:
pip install -r requirements.txt

## Create the network:
Use SUMO netedit tool to create a network and save it in the maps folder.

cd into maps folder and run the following command:

python randomTrips.py -n network.net.xml -r routes.rou.xml -e 300

This will create a routes.rou.xml file for 300 simulation steps for the network.

## Set configuration file:
Use the following command:
<net-file value='maps/city1.net.xml'/> <route-files value='maps/city1.rou.xml'/> </input>

## Train the model:
Use the following command:
python train.py --train -e 50 -m model_name -s 500

## Run the model:
python train.py -m model_name -s 500

## For running on Arduino:
For running Arduino for testing use --ard.

python train.py -m model_name -s 500 --ard

## Output:



https://github.com/Navtegh/Traffic-Light-Management-system-using-RL-and-SUMO/assets/25746677/3aa29862-e0cd-4214-b4b7-55e552089042





