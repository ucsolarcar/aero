# aero8
General CFD setup for OpenFoam v8  
  
## Instructions
- Move triSurface geometry to /constant/triSurface/  
- triSurface file must be in stl format and named "car.stl"  
.  
- Make any changes to setup.  
- Run commands in this order:  
	blockMesh  
	surfaceFeatures  
	snappyHexMesh -overwrite  
	simpleFoam  

## Default Setup
blockmesh:
	x			-5 to 15
	y			0 to 7
	z			-6 to 6
flow velocity			(25 0 0) m/s  
pressure			0 Pa  
turbulenceKE			0.24  
turbulentOmega			1.78  
.  
nu (kinematic viscosity)	1.5e-05 m^2/s  
.  
turbulence			off  
print force coeffs		on  
	centre of rotation	(2.5 0 0)


