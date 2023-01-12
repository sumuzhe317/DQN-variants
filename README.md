# RL-middle-hw
This is the repository for our AI-FinalHomework. It includes our every version of codes for Deep Q-Learning Network (DQN).

It includes Prioritized Experience Replay, Dueling DQN, Double DQN, Dueling-Double DQN and Human act.

You can run the below command to prepare for the environment:

```bash
python3 -m venv AI-Final
source AI-Final/bin/activate
python3 -m pip install -r requirements.txt
```

Remeber that every time you want to run the python code, you need to activate the virtual environment.

```bash
source AI-Final/bin/activate
```

You can change directory to the relative subfoloder, and run it.

```bash
cd Dueling-Double
python3 main.py
```

Note that you can change the hyperparameters to train you own agent:

```bash
python main.py -h
```

```bash
usage: main.py [-h] [--gamma [GAMMA]] [--seed [SEED]] [--memory_size [MEMORY_SIZE]] [--stack_size [STACK_SIZE]] [--eps_start [EPS_START]] [--eps_end [EPS_END]]                      
               [--eps_decay [EPS_DECAY]] [--render [RENDER]] [--batch_size [BATCH_SIZE]] [--policy_update [POLICY_UPDATE]] [--target_update [TARGET_UPDATE]]                         
               [--warm_steps [WARM_STEPS]] [--max_steps [MAX_STEPS]] [--evaluate_freq [EVALUATE_FREQ]] [--save_folder [SAVE_FOLDER]] [--load_folder [LOAD_FOLDER]]                   
               [--cuda_device [CUDA_DEVICE]] [--rew_path [REW_PATH]]                                                                                                                 
                                                                                                                                                                                     
optional arguments:                                                                                                                                                                  
  -h, --help            show this help message and exit                                                                                                                              
  --gamma [GAMMA]       decay rate                                                                                                                                                   
  --seed [SEED]         the seed to init weight                                                                                                                                      
  --memory_size [MEMORY_SIZE]                                  
                        store the memory
  --stack_size [STACK_SIZE]
                        store the relative frame's num
  --eps_start [EPS_START]
                        start of the eps
  --eps_end [EPS_END]   end of the eps
  --eps_decay [EPS_DECAY]
                        decay rate to run
  --render [RENDER]     render the training
  --batch_size [BATCH_SIZE]
                        every train batch's size
  --policy_update [POLICY_UPDATE]
                        the freq to update the policy DQN
  --target_update [TARGET_UPDATE]
                        the freq to update the target DQN
  --warm_steps [WARM_STEPS]
                        warm the agent and not to train
  --max_steps [MAX_STEPS]
                        the all steps
  --evaluate_freq [EVALUATE_FREQ]
                        the freq to evaluate and store the model
  --save_folder [SAVE_FOLDER]
                        where to store the evaluate model
  --load_folder [LOAD_FOLDER]
                        where to load the pre-trained model
  --cuda_device [CUDA_DEVICE]
                        use which GPU
  --rew_path [REW_PATH]
                        the path of rewards.txt
```