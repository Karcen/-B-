### 菜鸡一枚，不喜勿喷 🐔✨  
### Just a noob here, please be gentle! 🐥💫  

**仅供参考，肯定是错的**  
**For reference only - guaranteed to have flaws!**  

**抄我的必然拿不了奖**  
**Copying this = zero chance of winning!**  


### Dynamic Game Model: Sino-US Trade War Simulation System 🤝💹🌐

This project constructs a dynamic model of the Sino-US trade war based on evolutionary game theory. Implemented in Python, it simulates the multi-dimensional strategic interactions and dynamic parameter adjustments, offering insights into the evolution from confrontation to cooperation in trade conflicts. The model integrates factors such as technological competition, global value chain restructuring, and policy interventions to provide a quantitative analysis framework for understanding great power games.


### Key Model Features

1. **Strategy Space & Payoff Matrix**
   - 8 strategies each for China and the US (tariff adjustments, tech innovation, industrial subsidies, etc.)
   - 5 major industry sectors (High-Tech, Manufacturing, Agriculture, Services, Energy)
   - Dynamic payoff matrices modulated by technological progress, GVC positions, and international environment

2. **Dynamic Parameter System**
   - Policy intervention intensity decays over time ("war fatigue" effect)
   - Sector weights evolve according to industrial升级 trends (High-Tech +1% annually)
   - International environment includes economic cycles, third-party alliances, and sudden shocks
   - Technological progress forms positive feedback loops with strategic choices

3. **Evolutionary Mechanisms**
   - Strategy evolution based on replicator dynamics equations
   - Dual drivers of policy guidance and market selection
   - Integrated effects of inter-sector influences and random shocks


### Main Modules & Functions

1. **Parameter Initialization**
   - Define strategy sets, sector classifications, and base parameters
   - Generate randomized initial conditions for result diversity

2. **Dynamic Parameter Functions**
   - `get_dynamic_mu()`: Calculate policy intervention intensity
   - `get_dynamic_sector_weights()`: Adjust sector importance
   - `get_dynamic_international_environment()`: Simulate global economic factors
   - `get_dynamic_technology_impact()`: Model technological progress
   - `get_dynamic_global_value_chain_impact()`: Assess GVC restructuring

3. **Core Solver**
   - ODE integration using scipy.integrate.odeint
   - Handles high-dimensional, non-linear strategy evolution systems

4. **Visualization**
   - 8-panel plots showing strategy dynamics, payoffs, sector weights, etc.
   - Time-series analysis revealing long-term evolutionary trends


### Usage Instructions

1. **Environment Setup**
   ```bash
   pip install numpy matplotlib scipy
   ```

2. **Run Simulation**
   ```python
   python trade_war_simulation.py
   ```

3. **Customization**
   - Modify `BASE_PAYOFF_C/U` to adjust initial interaction effects
   - Tweak sensitivity parameters (e.g., `TECH_BASE_INNOVATION_SENSITIVITY`)
   - Customize policy trajectories in `get_policy_C/U` functions


### Output Interpretation

![Simulation Results](main.png)

1. **Strategy Evolution** 📈  
   Probability changes of key strategies over time for both countries

2. **Payoff Comparison** 💹  
   Average payoffs and total welfare dynamics

3. **Sector Weight Dynamics** 🏭  
   Evolution of industry importance in the global economy

4. **Policy Intensity** 🛠️  
   Decay of policy intervention effectiveness over time

5. **International Environment** 🌍  
   Impact of global factors on the trade war

6. **GVC Restructuring** 🔄  
   Shifts in global value chain positions for key sectors

7. **Technological Competition** 🚀  
   Tech progress comparison in high-tech sectors

8. **Policy Volatility** 📊  
   Uncertainty levels in strategic decision-making
