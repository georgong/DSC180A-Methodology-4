**Name:** Zhenghao Gong  
**Email:** z3gong@ucsd.edu  
**Section:** From Data to Dispatch - Optimizing SDG&E Field Services
**Mentor:** Phi Nguyen, Chuck Hahm, Fatemeh Aarabi
---

### **1. What is the most interesting topic covered in your domain this quarter?**
The most interesting topic in our domain has been **data-driven optimization of operational scheduling** for the SDG&E Gas Department.  Our dataset captures real maintenance activities — task creation times, assigned crews, completion timestamps, and spatial distribution.  Unlike typical classroom data, this one exposes the friction between planning and execution: how human behavior, time constraints, and geographic coverage all influence efficiency.  It shows how data science can interact directly with real-world logistics, where every prediction can translate into fewer delays and safer operations.


### **2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**
In Quarter 2, I would like to extend our analysis toward a delay-risk prediction and scheduling optimization system.  The idea is to predict, for each incoming task, the probability of delay given contextual factors such as crew workload, time of day, district, and task type.  Once we can estimate those risks reliably, the next step would be to simulate alternative scheduling orders or re-assignment strategies that minimize total downtime.  This approach blends predictive modeling with operational decision support — moving from describing inefficiency to actively improving it.


### **3. What is a potential change you’d make to the approach taken in your current Quarter 1 Project?**
Our Quarter 1 work focused on exploratory analysis and descriptive statistics.  If I could redesign that stage, I would incorporate causal inference and temporal analysis much earlier.  For example, instead of only observing that morning assignments tend to finish faster, I would test whether the assignment time *causally* affects task duration after controlling for crew experience and task type.  Similarly, I would model time-series dependencies between consecutive tasks performed by the same crew — turning static snapshots into evolving operational patterns.  These changes would help shift the analysis from correlation-based insight to actionable evidence.


### **4. What other techniques would you be interested in using in your project?**
I would like to explore graph-based learning and temporal modeling techniques to capture the complex relationships and time-dependent nature of our scheduling data. Each task in the SDG&E system is connected to specific crews, districts, and time windows, and these form a naturally structured network. Traditional tabular models treat each task independently, but a graph neural network (GNN) could model how information flows between related tasks — for example, when the same crew performs similar tasks, or when consecutive tasks in the same area influence one another. By extending this to a heterogeneous and temporal graph, the model could also represent (1) how performance changes over time, (2) which crews specialize in certain task types, and (3) how different task priorities (such as emergency or investigation tasks) affect scheduling outcomes. The attention mechanisms in modern GNNs could help the model automatically focus on high-priority or time-critical connections, reflecting how human schedulers think under constraints.Ultimately, such a model could predict not just whether a task will be delayed, but why — by analyzing its position and dependencies in the operational network — paving the way toward more adaptive, context-aware scheduling optimization.

