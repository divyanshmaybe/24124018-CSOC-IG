# Reinforcement Learning Projects

This directory contains reinforcement learning implementations exploring various algorithms on custom environments.

## Week 2 Projects

### 1. Frozen Lake Environment (`Week2/FrozenLake/`)

**Algorithms Implemented:**
- **Monte Carlo**: Model-free learning using episode returns
- **SARSA**: On-policy TD learning
- **Q-Learning**: Off-policy TD learning
- **Policy Iteration**: Model-based policy improvement
- **Value Iteration**: Model-based value function optimization

**Environments:**
- **8x8 Frozen Lake**: Custom grid with holes, stochastic slippery movement (20% slip probability)
- **Large Frozen Lake**: 26x10 complex grid with multiple holes and goals

**Key Features:**
- Custom Gymnasium environments with stochastic transitions
- Comparative analysis across different algorithms
- Performance evaluation on multiple environment sizes
- Reward smoothing and convergence analysis

**Files:**
- `task.ipynb`: Main implementation with all algorithms and experiments
- `rl2.ipynb`: Focused implementation of Policy and Value Iteration
- `reinforcement_learning_report.pdf`: Comprehensive analysis report
- `task_1_and_2_derivation_and_proofs.pdf`: Mathematical derivations and proofs

### 2. Cliff Walking Environment (`Week2/CliffWalking/`)

**Algorithms Implemented:**
- **SARSA**: On-policy temporal difference learning
- **Q-Learning**: Off-policy temporal difference learning
- **Double Q-Learning**: Variance reduction technique for Q-Learning

**Environment:**
- Custom Cliff Walking grid (5x20) with:
  - Starting position at bottom-left
  - Goal at bottom-right
  - Cliff area with -100 reward (falls reset to start)
  - Standard moves with -1 reward

**Key Features:**
- Custom environment implementation with stochastic action execution
- Comparative performance analysis
- Training reward visualization

**Files:**
- `bonus_task.ipynb`: Complete implementation and analysis

## Common Features Across Projects

### Environment Characteristics
- Custom Gymnasium-compatible environments
- Stochastic action execution (configurable slip probabilities)
- Terminal states with appropriate rewards
- Observation spaces and action spaces properly defined

### Algorithm Implementations
- Epsilon-greedy exploration with decay schedules
- Proper convergence criteria
- Reward tracking and analysis
- Policy extraction from learned value functions

### Evaluation Metrics
- Average reward per episode
- Average episode length
- Training time comparison
- Convergence analysis

## Usage

1. Install dependencies: `pip install -r ../requirements.txt`
2. Navigate to specific project directory
3. Open notebooks in Jupyter Lab
4. Run cells sequentially to train and evaluate algorithms

## Dependencies

- numpy
- gymnasium
- matplotlib
- jupyter

## Results Summary

### Frozen Lake Experiments
- **Model-based methods** (Policy/Value Iteration) show fast convergence but require environment model
- **Model-free methods** (Monte Carlo, SARSA, Q-Learning) learn directly from experience
- **Q-Learning** generally performs well on stochastic environments
- **Performance scales** with environment complexity

### Cliff Walking Experiments
- **Double Q-Learning** reduces overestimation bias compared to standard Q-Learning
- **SARSA** shows more conservative behavior due to on-policy learning
- **All methods** successfully learn optimal policy avoiding the cliff

## Mathematical Foundations

The implementations are based on standard reinforcement learning theory:
- Markov Decision Processes (MDPs)
- Bellman equations
- Temporal Difference learning
- Policy and Value iteration algorithms

See `task_1_and_2_derivation_and_proofs.pdf` for detailed mathematical analysis.

## Author

Divyansh Maybe (Roll Number: 24124018)
