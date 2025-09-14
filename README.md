# Connect-4-AI-agent
This project aimed to develop a competitive AI agent for Connect 4, exploring and implementing several AI techniques.  
We implemented a Monte Carlo Tree Search (MCTS) algorithm, enhancing its performance through memory caching and neural network-based move biasing. Both Fully Connected (FCNN) and Convolutional Neural Networks (CNN) were trained and integrated with the MCTS agent. Performance evaluation was conducted against baseline agents and through self-play.  
The entire project can be accessed at the following link https://colab.research.google.com/drive/15EcWhbR69FXOAV37s3VFs66QXllsVwu4?usp=sharing  

## Overview
In this project, we implemented:

- **Neural network models (FCNN and CNN)**  
  These models are trained and validated on a pre-existing dataset by converting the game board representation and moves into PyTorch tensors. After training the models on the pre-existing dataset, given a game scenario, the neural networks are able to predict the best move to make.

- **Three variants of the Monte Carlo Tree Search (MCTS) decision-making algorithm:**  
  1. **Basic MCTS Agent** – The agent makes decisions solely based on the standard MCTS algorithm.  
  2. **MCTS with Memory Cache** – This version includes a cache to store and reuse previously analyzed game scenarios, improving efficiency.  
  3. **MCTS Guided by Neural Networks** – The predictions from the previously mentioned neural networks are used to guide the MCTS algorithm.  
     This helps focus on more promising game scenarios, leading to smarter and more efficient decisions.

  > This iterative process resulted in the development of an agent that is highly efficient both computationally and strategically.

- **Three AI Bots**  
  These were created to evaluate the performance of the different models and approaches.

- **Elo Tournament**  
  An Elo rating system was implemented to compare and rank the different bots' performance.

- **Final Report**  
  A detailed report analyzing the tools used and the results obtained throughout the project.

---

## Technical Details
The project is written in **Python** and primarily developed on **Google Colab** to simplify collaborative development and sharing.  

To access and run the project:
1. Open the file [`ML_final.py`](ML_final.py).
2. The file contains:
   - The **Connect Four game engine** implementation.  
   - The **dataset** used to train the neural networks.  
   - The code for the **bots**, built using different machine learning architectures and MCTS variants.

---

## Responsibilities and Contributions
The **Connect Four game engine** code was provided by **Professors Giovanni Paolini and Stefano Pagliarani**.  
The **machine learning architectures** were designed and implemented by **Antony Di Pietrantonio**, **Jacopo Elefante**, **Kevin Mazzotti**, and **Michele Priolo**.

After an initial phase of problem analysis and solution design, the work was divided as follows:

### **Antony Di Pietrantonio**
- Refactored and optimized the implementations of both the MCTS algorithms and the game engine.  
- Developed the **Elo rating system** to evaluate and compare agent performance.

### **Jacopo Elefante**
- Led the **core development of the MCTS algorithms**.  
- Created various **AI agents (bots)** based on these algorithms.

### **Kevin Mazzotti**
- Designed and implemented the **evaluation and simulation framework**.  
- Developed mechanisms to:
  - Assess the performance of different agents.  
  - Run simulations to gather performance data.  
  - Analyze results to compare the effectiveness of different strategies and model configurations.

### **Michele Priolo**
- Designed and implemented the **neural network architectures (FCNN and CNN)**.  
- Trained and evaluated the models, tuning various parameters to identify the most effective configurations.

---

## Key Features
- PyTorch-based **neural networks** for game state evaluation.
- Multiple **MCTS algorithm variations**.
- **Elo ranking system** for objective performance comparison.
- Fully modular and extensible codebase.

---

## How to Run
1. Open the project in **Google Colab** or your local Python environment.
2. Run the [`ML_final.py`](ML_final.py) script.
3. Follow the prompts to:
   - Train the neural networks.
   - Run simulations between bots.
   - Analyze performance using the Elo rating system.

---

## License
This project is for educational purposes and is part of a university assignment.  
Please refer to the repository's LICENSE file for more details.
