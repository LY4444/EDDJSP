# MAEDQN for EDDJSP
# # Introduction
  Dear readers, thanks you for your visit. This repository would shares the full code of the paper ''Multi-objective Optimization of Energy-Efficient Dynamic Distributed Job Shop by Multi-agent Expected Deep Q-network'' after it is accepted by the reviewing jounal. Meanwhile, through preliminary research and communication recently, we have established an initial cooperation intention with Zoomlion (Changsha, China) to verify the superiority of our method in real-world. The progress and results would be successively updated.
# # # Description of these codes
1. Energy_efficient_distributed_job_shop.py. It establishs a energy-efficient distributed job shop environment, contains the updating function of state features, the action functions of G-agent, S-agent and D-agent, and the scheduling function for the selected job and factory.
2. MAEDQN.py. It creats a EDQN class with a experiance replay buffer and a target network. Grounded in this, a MAEDQN-based dynamic scheduling framwork is established.
3. Objection_for_EDDJSP.py. It contains a Object class and its data updating function.
4. Job_creator.py. It is responsible for generating instance for the training and testing experiments.
5. Composite_rule.py. It encompasses a evaluate function for all composite rules, which would calculate and save the objectives of each composite rules autmaticlly.
6. Energy_efficient_distributed_job_shop_P.py. It have the identical structure with the "Energy_efficient_distributed_job_shop.py", but contains all priority dispatching rule.
7. Priority_dispatching_rule.py. It owns the same structure and function with ''Composite_rule.py''.
8. EDQN.py, MADQN.py, MADDQN.py, MADRL_C.py, MADRL_W.py, MADRL_H.py. They are the comparative algorithms in Section 6.3.3.
# # # Procedure of using above codes
1. To train and test the MAEDQN, MAEDQN.py is employed and all key parameters can be modified here.
2. To conduct the comparative experiment of Section 6.3.1, the composite_rule.py is employed.
3. To implement the comparision in Section 6.3.2, the Priority_dispatching_rule.py is used.
4. For the section
