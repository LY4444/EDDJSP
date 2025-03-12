# MAEDQN for EDDJSP
# # Introduction
  Dear readers, thank you for your esteemed visit. This repository will share the full code of the paper ''Multi-objective Optimization of Energy-Efficient Dynamic Distributed Job Shop by Multi-agent Expected Deep Q-network'' after it is accepted by the reviewing journal. In the following section, we will describe the content of these code files in detail.
# # # Description of code files
# # # # Code files in the folder ''drl''
1. Energy_efficient_distributed_job_shop.py. It is used for establishing an energy-efficient dynamic distributed job shop scheduling environment. This environment contains the updating function of state features, the action functions of G-agent, S-agent, and D-agent, and the scheduling function.
2. Objection_for_EDDJSP.py. It is used for creating job and machine objects and contains their data updating functions.
3. Job_creator.py. It is responsible for generating instances under different production configurations.
4. MAEDQN.py. It contains an EDQN class with an experience replay buffer and a target network. Grounded in this, a MAEDQN-based dynamic scheduling framework is established. At the end of this file, the ''argparse'' is employed to convenient the parameter setting.
5. Composite_rule.py. It encompasses an evaluate function for all composite rules, which would calculate and save the results of composite rules.
6. Energy_efficient_distributed_job_shop_P.py. It has a structure similar to the "Energy_efficient_distributed_job_shop.py", but contains all combined priority dispatching rules (PDRs).
7. Priority_dispatching_rule.py. It owns the similar structure and function with ''Composite_rule.py'' and is utilized for evaluating combined PDRs.
8. As for other code files namely MADQN.py, MADDQN.py, MARL_C.py, MARL_W.py, MARL_H.py, they are the comparative algorithms in Section 6.3.3.
# # # # Code files in the folder ''metaheuristics''
1.Energy_efficient_distributed_job_shop_Luo. It is used for establishing an energy-efficient dynamic distributed job shop scheduling environment. This environment contains the information updating function. The structure and function of Energy_efficient_distributed_job_shop_Gong.py is similar to it.
2. Encode_Luo.py and Encode_Gong.py. They contain the ''encode'' class and are used for generating the initial population.
3. Decode_Luo.py and Decode_Gong.py. They include the ''decode'' class and are responsible for decoding the chromosomes of the population. 
4. Job_Luo.py and Job_Gong.py. They are used for creating the job objects and contain the functions for inputting and deleting information.
5. Machine_Luo.py and Machine_Gong.py. They are used for creating machine objects and contain the functions for inputting and deleting information.
6. Job_creator.py. It is responsible for generating instances under different production configurations.
7. FastNDSort.py. It provides non-dominated sorting for solution sets.
8. MA_Luo.py and MA_Gong.py. They contain the memetic algorithm class, fitness calculation functions, crossover functions, mutation functions, and local search functions.
9. KTMA_Luo.py. It is the main algorithm for rescheduling.
10. IMA_Gong.py. It is the main algorithm for rescheduling.
