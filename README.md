# MVC_2025
Repository of the 2025 IEEE VTS Motor Vehicle Challenge (MVC). Please refer to the [INSTALLATION.md](INSTALLATION.md) file for instructions about how to use the software and the necessary software requirements.
The website of the challenge is [here](https://vtsociety.org/event/meeting/ieee-vts-motor-vehicles-challenge-2025).

## Introduction
![VPPC2024_MVC2025_Fig01c](https://github.com/user-attachments/assets/3058258b-4cb9-44c9-a135-982c7fad2200)

The topic of the challenge is to develop an <mark>Energy Management System</mark> (EMS) for a tugboat application. The tugboat powertrain consists of a dual-three phase permanent magnet synchronous motor where each of the two three phase windings are fed by a three phase inverter. The power source of each inverter is different, that is the following two energy sources are employed:
* a battery pack (BP)
* a supercapacitor module (SM)

## Submission of proposal
[SUBMISSION LINK](https://forms.gle/N4LjFR53m6wfZPHh6)

The proposal(s) must be submitted by using the above link. The deadline for the proposal submission is :red_circle:<mark>24th of March, 2025</mark>:red_circle: : <ins>this is a hard deadline, it will not be postponed further.</ins>

For safety reasons, the submission can be made only by people with a Gmail account. In the form, it is possible to indicate the academic/industrial contact. If the possession of a Gmail account is an issue, please contact MVC 2025 organizers.


## Rules
The participants to the challenge will operate only in the EMS block provided within the simulation file. All the remaining blocks must not be modified. <ins>The final evaluation will be carried out by implementing the EMS block developed by each participant in the original simulation file</ins>. That is, <mark>all the modifications made in subsystems which are not the EMS one will be discarded</mark>. 

Important rules that the submitted proposal must satisfy for being considered valid in this competition
1. All parameters defined in the "Parameters" folder can be used to develop the strategy.
2. All parameter defined in the "Reference" folder and "main_runSimulation.m" **cannot** be used to develop the strategy: the EMS **must not** adopt whatsoever a priori knowledge of the reference working cycle.
3. All parameters adopted for the developed strategy **must** be specified only in the "ProposedEMS.m" script.
4. Energy constraints of the BP and SM must always be guaranteed.

## What has to be uploaded for evaluation
In order to evaluate each proposal, the teams must submit in the form [SUBMISSION LINK](https://forms.gle/N4LjFR53m6wfZPHh6) a unique compressed file (.zip or .rar extension) containing only the following files:
- "proposedEMS.m" renamed as "nameTeam_numProp_EMS.m" where "numProp" must identify the proposal number of the team. If only one proposal is presented, please use "num1" (e.g., "teamWhite_prop1_EMS.m"). Please avoid spaces in the file name.
- simulink subsystem of the proposed EMS. Rename the file as “nameTeam_numProp_Simulink.slx”. The same considerations made for the EMS Matlab script holds. Please note that **only** the Simulink block of the EMS is necessary, not the whole simulation. It is mandatory to adopt the same names of the signal in the Simulink buses.

## Release Notes
Please refer to the [CHANGELOG.md](https://github.com/VTSociety/MVC_2025/blob/main/CHANGELOG.md) file for modifications of the simulation and differences with respect to the paper in the [Bibliography](), that is [10.1109/VPPC63154.2024.10755298](https://ieeexplore.ieee.org/document/10755298) ([preprint version here](Materials)).

Remarks:
* Please take notice of the [Discussion board](https://github.com/VTSociety/MVC_2025/discussions) for Q&A. Start a new discussion if you've found no answer to your issue. No answers will be given to questions related the MVC 2025 by private emails.

## Bibliography
M. Porru, A. Serpi, F. Tinazzi and L. Ortombina, "IEEE VTS Motor Vehicle Challenge 2025 – Energy Management and Control of a Marine Electric Propulsion System," 2024 IEEE Vehicle Power and Propulsion Conference (VPPC), Washington, DC, USA, 2024, pp. 1-6, doi: [10.1109/VPPC63154.2024.10755298](https://ieeexplore.ieee.org/document/10755298).

## License
All files of the repository "MVC 2025" are intended solely for the aim of the Motor Vehicle Challenge competition organised within the IEEE VTS Society. The Authors declined all responsabilities for usage outside this context. 

Copyright © 2024-2025. The code is released under the [CC BY-NC 4.0 license](https://creativecommons.org/licenses/by-nc/4.0/legalcode). Link to [short summary of CC BY-NC 4.0 license](https://creativecommons.org/licenses/by-nc/4.0/). For attribution see also [license file](LICENSE.md).


