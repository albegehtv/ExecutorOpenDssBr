# ExecutorOpenDss
This project is a C# [OpenDSS](http://smartgrid.epri.com/SimulationTool.aspx) customization to batch calculate the power flow of brazilian eletric distribution feeders. The project main objective is calculate energy and power losses. The feeder \*.dss files (see FeederExample directory) are very similar to the ones created by the brazilian regulatory agency [ANEEL](http://aneel.gov.br/) program (GeoPerdas.exe). In fact, the files are created from the same database (**GeoPerdas**), using a FME project (see item 3 below).

There are 3 directories in this project:
1. **ExecutorOpenDssBr**: the C# project. As it is a complete Visual Studio project, there wont be any dificult to compile it.
You'll have to only set up the local path of 2 resources directories:
"*Caminho dos arquivos dos alimentadores \*.dss*", thats is the FeederExample path.
"*Caminho dos recursos permanentes*", thats is the "global" resources files.

The project also uses 2 dll files: EEPlus.dll (some Excel stuff) and Auxiliares.dll (the co author Daniel Rocha routines) already included in the project.    

2. **FeederExample**: a 13.8kV feeder *.dss files. There are also some xlsx and txt files with external information necessary to the the "ExecutorOpenDssBr" run *.dss files. I'll explain more about this part soon.  

A lot of code optimization can be done in this project, so any help is welcome. The code comments are in portuguese (sorry for non-portuguese natives).

Ezequiel C. Pereira
