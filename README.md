# shinyenet-app
The objective of the Shinyenet application is to simulate the gasification processes involved in converting communal waste into valuable resources. Communal waste primarily comprises organic materials like biomass and combustibles from both household and industrial sources. Through gasification, this waste is transformed into synthetic gas, known as syngas. The composition of syngas is heavily influenced by factors such as the temperature within the gasification chamber and the makeup of the waste materials.

The primary target within syngas production is hydrogen, a versatile resource capable of generating electrical energy via fuel cells. Additionally, syngas contains other valuable components such as methane and carbon monoxide, which can serve various purposes. These include direct combustion for heating or electricity generation.

The application also incorporates the use of electrolyzers to produce hydrogen from electricity. This reverse mode enhances operational flexibility of the simulated facility to meet diverse energy demands.

In addition to gasification, the application can simulate the process of pyrolysis, which is mainly used for the production of liquid fuel.

## Gasification
The gasification process has 3 main parameters - nozzle base constant, plasma torch power, and filling pressure. These can be adjusted using sliders on the top of the tab. The fourth parameter that can be adjusted in this section is the amount of waste introduced into the system.

### Plasmatron
This tab displays temperature and normalized temperature computed from the given parameters.

### Gasification chamber
The main part of the gasification process takes place in the gasification chamber. In this tab, parameters of the gasification process are displayed. The user can choose between the models of symbolic or polynomial regression and compute the amount of syngas produced and its composition.

### Hydrogen tank filling
The hydrogen produced in the gasification chamber is stored in hydrogen tanks. The user can adjust the pressure, volume and temperature of the tanks to see how long does it take to fill up the tank.

### Combustion
Combustion is an alternative way to produce energy from hydrogen. It operates only when fuel cells are shut down or their capacity is not enough to use up all the hydrogen available. For the simulation, the user can choose the amount of hydrogen used in combustion, and parameters of the process as efficiency and heating value.

### Fuel cell
Producing energy from hydrogen in fuel cells is the main process. Parameters as efficiency, heating value, number of fuel cells and their power can be adjusted. The main output us the electrical energy obtained.

### Electrolyzer
Electrolyzers work in reverse to the fuel cells, producing hydrogen from water and electricity. The amount of energy obtained from photovoltaics and from the grid can be adjusted, and the amount of hydrogen produced is displayed.

### Photovoltaics and wind turbine
Photovoltaic panels and wind turbines provide electricity to the battery and electrolyzer. Parameters such as photovoltaics power, wind turbine power and battery capacity can be chosen. Outputs of the system - energy used by electrolyzer, energy sent to battery or grid from photovoltaics, wind turbine, or a fuel cell, and time to fill up the battery - can be seen on this tab.

## Pyrolysis
Pyrolysis is a process to produce liquid fuel in the facility. The adjustable parameters are energy and the amount of waste introduced into the system. The results are the amounts of liquid fuel, gas, and biochar. The composition of the gas, which is a byproduct of this process, is given.

## Optimization
In this tab, the user can choose between two objectives - maximization of the volume of hydrogen in gasification, or the amount of liquid fuel in pyrolysis. For gasification, one or more of the three parameters can be chosen to remain fixed on a specified value. By clicking the Start optimization button, a set of the found parameters is displayed, and it is possible to choose to use the optimized values of the parameters, or reset the optimization.
