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

## Pyrolysis


## Optimization
