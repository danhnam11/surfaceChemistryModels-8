# surfaceChemistryModels-8

## General Information
A package for simulations of reacting flows using surface reactions in OpenFOAM 8.0. 
In this package, a new library, _surfaceChemistryModels_, is developed for handling several types of commonly used surface reaction rate constant models such as the basic Arrhenius form, sticking coefficient, and surface coverage dependence models. A new solver, _porousPBRFoam_, is developed for simulations of catalytic packed bed reactors using porous media model with detailed surface chemical mechanisms.

## Installation
- Since this solver is developed based on OpenFOAM 8.0 in Linux operating systems, the complete installation of OpenFOAM 8.0 framework is required. 
- Prepare a directory on your system, e.g., _yourDirectory_:

		mkdir ~/OpenFOAM/yourDirectory/
		cd ~/OpenFOAM/yourDirectory/	
- Download source files using git: 

		git clone https://github.com/danhnam11/surfaceChemistryModels-8.git

- Specify the path of your _src_ directory to an environment variable, _LIB_porousCAT_SRC_. For example:

		echo "export LIB_porousCAT_SRC=~/OpenFOAM/yourDirectory/surfaceChemistryModels-8/src/" >> ~/.bashrc
		source ~/.bashrc
- To compile the necessary libraries and solver, go to _surfaceChemistryModels-8_ directory and run the _Allwmake_ script:

		cd ~/OpenFOAM/yourDirectory/_surfaceChemistryModels-8/
		./Allwmake

- Now all necessary libraries inlcuding _surfaceChemistryModels_ library (for handling surface reactions), and a solver _porousPBRFoam_, are stored at _$FOAM_USER_LIBBIN_ and _$FOAM_USER_APPBIN_ directory. These newly compiled libraries, solvers, and utilities are ready to be used.

- To remove all compiled libraries and solvers, go to _surfaceChemistryModels-8_ directory and run the _Allwclean_ script:

		cd ~/OpenFOAM/yourDirectory/_surfaceChemistryModels-8/
		./Allwclean

## Using this package 
- Upon completing the compilation process, the solvers can be utilized by simply typing _porousPBRFoam_ in the terminal. All important instructions for utilizing _surfaceChemistryModels_ library and for case setting can be found in _tutorial_ directory. 
- Readers are referred to our paper for all validation data.

## Tutorials
Tutorials for catalytic packed bed reactor test case is available in the _tutorial_ directory.

	cd ~/OpenFOAM/yourDirectory/surfaceChemistryModels-6/tutorials/

## Authors 
This package was developed at Clean Combustion & Energy Research Lab., Dept. of Mech. Engineering, Ulsan National Institute of Science and Technology (UNIST), Korea (Prof. C.S. Yoo: https://csyoo.unist.ac.kr/). If you publish results that are obtained using this package, please cite our papers as follows:
- D. N. Nguyen, Jae Hun Lee, C. S. Yoo, surfaceChemistryModels: A new library for simulations of reacting flows using surface reactions in OpenFOAM, Computer Physics Communications (2024)(in preparation).

Contact:
- danhnam11@gmail.com or nam.nguyendanh@hust.edu.vn 
