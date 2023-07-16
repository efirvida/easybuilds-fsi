# easybuilds-fsi

Easybuild files to setup and FSI simulation environment with
preCICE+OpenFOAM+CalculiX on HPC system that uses easybuild as module manager


to install:

	$ eb --robot=$PWD ./preCICE-2.5.0-foss-2022a-Python-3.10.4.eb \
	   ./preCICE_CalculiX-2.20.0-foss-2022a-CCX-2.20-preCICEv2.5.0.eb \
	   ./preCICE_OpenFOAM-1.2.0-foss-2022a-OFv10-preCICEv2.5.0.eb

Then just use:

on fluid machine:

	$ module load preCICE_OpenFOAM
	$ . $FOAM_BASH

on solid machine:

	$ module load preCICE_CalculiX
