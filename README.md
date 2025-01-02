# Research_agent_Crewai(**Latest AI Development Crew**)

This repository showcases a **CrewAI-based project** designed for automating research and reporting on topics related to **AI Language Learning Models (LLMs)**. The system leverages structured tasks, agent configurations, and a local LLM model (**OLLAMa 3.1**) to deliver insights and generate reports.

---

## **Features**
- **Agent-based Design**:
  - **Researcher Agent**: Gathers and analyzes data.
  - **Reporting Analyst**: Structures the findings and generates reports.
- **Task Automation**:
  - **Research Task**: Focuses on collecting and synthesizing AI-related developments.
  - **Reporting Task**: Summarizes research findings into a report (`report.md`).
- **Crew Integration**:
  - Facilitates collaborative processing of agents and tasks.
  - Offers sequential or hierarchical execution options.
- **Local LLM**:
  - Utilizes **OLLAMa 3.1** for efficient and private natural language processing.

---

## **Tech Stack**
- **CrewAI Framework**: Handles agent and task management.
- **OLLAMa 3.1**: Local LLM for secure and efficient language modeling.
- **Python 3.8+**: Core programming language.

---

## **Setup Instructions**

### 1. Clone the Repository
```bash
git clone <repository_url>
cd <repository_name>
```

### 2. Install Dependencies
Ensure Python 3.8+ is installed, then run:
```bash
pip install -r requirements.txt
```

### 3. Configure Agents and Tasks
Update the configuration files in the `config/` directory to customize agents and tasks:
- `agents.yaml`: Define the behavior and tools for the agents.
- `tasks.yaml`: Specify the tasks' details, including input and output structures.

### 4. Install OLLAMa 3.1
Ensure **OLLAMa 3.1** is installed and running locally. Follow [OLLAMa Installation Guide](https://ollama.ai/docs) for setup instructions.

---
### Installation of CrewAi Framework:
```bash
pip install 'crewai[tools]'
or
pip install crewai crewai-tools

pip install --upgrade crewai crewai-tools

#Veryify Installation
pip freeze | grep crewai


cd latest-ai-development
crewai install

# Command to run Agent:
Crewai run
```


---

## **Key Components**

### **Agents**
1. **Researcher Agent**:
   - Handles the research process using configurations from `agents.yaml`.
   - Verbose mode enabled for detailed logs.

2. **Reporting Analyst**:
   - Structures the data and generates reports.
   - Outputs data to `report.md`.

### **Tasks**
1. **Research Task**:
   - Processes research input and generates structured findings.

2. **Reporting Task**:
   - Uses research outputs to produce a report file.

### **Process Management**
The crew supports two process modes:
- **Sequential**: Executes tasks one after the other.
- **Hierarchical**: Supports dependent tasks and structured workflows.

---

## **Error Handling**
The system ensures robust error handling with clear exceptions:
- Missing or incorrect configuration files.
- Invalid arguments passed to CLI commands.
- Issues with task or agent execution.

---

## **Contributing**
Contributions are welcome! Feel free to submit issues or pull requests to improve the system.
c

---

## **Acknowledgments**
- **CrewAI Framework**: For providing a robust agent and task management platform.
- **OLLAMa Team**: For creating a versatile local LLM for natural language processing.
