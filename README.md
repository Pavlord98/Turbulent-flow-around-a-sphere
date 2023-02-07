# Turbulent-flow-around-a-sphere

This project is a continuation of my [laminar flow around a sphere project](https://github.com/Pavlord98/Laminar-flow-around-a-sphere).

## Pre-analysis

This set of simulations covers flows with Reynold's numbers ranging from 300 up to values close to the cricital value of the Reynold's number. I used RANS modelling, the K Omega SST model to be precise. This RANS model is the most popular and has proved to be a good choice for flows with adverse pressure gradients, especialy when compared to the K Epsilon model. 

RANS modells have been proved to be insufficient when dealing with modelling the drag crisis phenomenom, and because of this this set of simulations will deal with flows whose Reynold's number dosent exceed 3e5. 

## Geometry and Mesh

The geometry is the same as in the laminar project, but the meshes for the higher Reynold's number cases have been aditionally refined in order to obtain adequate values of y<sup>+</sup> on the sphere. Those meshes were refined by specifying higher refinements levels and adding more inflation layers to the sphere.

## Numerical model

Just like in the laminar project, I used the potentialFoam solver to obtain a good initial guess of the pressure and velocity fields. Unlike the laminar case, here I implemented the K Epsilon Omega SST model with the simpleFoam solver. 
For the boundary conditions for k and omega I used the recomendations from [here](https://turbmodels.larc.nasa.gov/sst.html).

## Results

All of the values are very close to the experimental values and thus I conclude that the simulations are accurate.


![DragCoefficientGraph(3)](https://user-images.githubusercontent.com/84512701/217218334-627b1b47-e63c-4b17-9239-1a6011ea22c1.png)
