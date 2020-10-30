## Mesa agent based modeling in python

I am going to talk about a data science method called Mesa. Mesa is an Apache2 licensed agent-based modeling framework in python (pypi.org). Mesa allows users to quickly create agent-based models using built in core components, such as spatial grids and agent schedulers or customized implementations (pypi.org). Mesa also allows users to visualize those components using a browser-based interface and analyze their results using python’s data analysis tools (pypi.org).

Mesa is not difficult to set up. It runs in the virtual environment by using the command “conda activate mesaenv” (towardsdatascience.com). It is possible to even install Mesa through the virtual environment by using “python3 -m pip install mesa” (towardatascience.com). Once those commands have been run by the termina Mesa is ready to run by the user.

Mesa is easy to run and set up but the model itself has many unique features. Mesa uses several agent schedules and requires the user to specify which one is being used (https://www.researchgate.net). Mesa also facilities live visualization (https://www.researchgate.net). This means that Mesa avoids issues of system-specific dependencies by using the browser as a front-end giving framework and model developers access to the full range of modern JavaScript data visualization tools. One other unique feature of Mesa is that it makes minimal assumption about the form of a model (https://www.researchgate.net). This is because models come in many shapes, so Mesa aims to offer as et of components that can be easily combined and extended to build different kind of models (https://www.researchgate.net).

The overall framework of Mesa can be broken to smaller section. Mesa’s modules can be divided into three overall categories: modeling, analysis and visualization (https://www.researchgate.net). The modeling components are the core of what is needed to build a model (https://www.researchgate.net). In this case it would a model class to store the model level parameters and serve as a container for the rest of the components (https://www.researchgate.net). Then an Agent class will describe the model’s agents and a scheduler will control the agent activation regime, and handle time in the model (https://www.researchgate.net). The scheduler also controls the components describing the space and network the agents are situated in (https://www.researchgate.net). The analysis components are the data collectors used to record data from each model run, and batch runners are for automating multiple runs and parameter sweeps. Finally, the visualization components are used to map from a model object to one or more visual representations using a server interface to a browser window (https://www.researchgate.net).



**Sources:**

      Foong, N. (2019, November 01). Introduction to Mesa: Agent-based Modeling in Python. Retrieved October 29, 2020, from https://towardsdatascience.com/introduction-to-mesa-agent-based-modeling-in-python-bcb0596e1c9a

      Kazil, J. (2015, January). Find and share research. Retrieved October 29, 2020, from https://www.researchgate.net/

      Kazil, J. (2020, May 5). Mesa. Retrieved October 29, 2020, from https://pypi.org/project/Mesa/
