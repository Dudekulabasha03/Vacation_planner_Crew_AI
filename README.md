# Vacation Planner 

Welcome to the VacationPlanner Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.13 installed on your system. This project uses [UV] for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/vacation_planner/config/agents.yaml` to define your agents
- Modify `src/vacation_planner/config/tasks.yaml` to define your tasks
- Modify `src/vacation_planner/crew.py` to add your own logic, tools and specific args
- Modify `src/vacation_planner/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the vacation_planner Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The vacation_planner Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.


............1. Pre-Requisites................

1. VSCode - https://code.visualstudio.com/download
2. Install Python ---> Recommended: 3.11.9 (3.10 to 3.13) - https://www.python.org/downloads/
3. Install AWS CLI --- > https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
4. Setup IAM Role for AWS CLI
5. Optional Step - Download C++ compiler for VSCode ---- > https://code.visualstudio.com/docs/cpp/config-mingw
....................................................................


......2. CrewAI Installation---> https://docs.crewai.com/installation................
pip install uv
uv --version
uv tool install crewai
uv tool list
uv tool update-shell (One time to set the path)
.......................................................................

.........3. Create Project............
crewai create crew vacation_planner
Select 8
Bedrock Model in .env  -----> Should have access to Model (Check from console)
Set Access Key, Secret Key, region-us.west-2
Update Agent and Task details in YAML
Add Tools to Agents in Crew.py 
Update Agent and Task details in Crew.py
Add input in main.py

...........Run the Project.....................
Lock dependencies --- > crewai install (uv lock file)
uv add boto3
Run Command --- > crewai run
............................................

# Vacation_planner_Crew_AI
