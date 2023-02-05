# Turbulent-flow-around-a-sphere

This project is a continuation of my [laminar flow around a sphere project](https://github.com/Pavlord98/Laminar-flow-around-a-sphere).

## Pre-analysis

This set of simulations covers flows with Reynold's numbers ranging from 300 up to values close to the cricital value of the Reynold's number. I used RANS modelling, the K Omega SST model to be precise. This RANS model is the most popular and has proved to be a good choice for flows with adverse pressure gradients, especialy when compared to the K Epsilon model. 

RANS modells have been proved to be insufficient when dealing with modelling the drag crisis phenomenom, and because of this this set of simulations will deal with flows whose Reynold's number dosent exceed 3e5. 
