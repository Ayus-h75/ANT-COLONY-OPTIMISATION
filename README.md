# ACO Path Navigator  

An innovative approach to path planning using Ant Colony Optimization (ACO) for 2D environments with barriers, featuring intelligent backtracking, ACO-Dijkstra fusion, and self-adjusting parameters.  

## Key Features  

- **Dynamic Environment Setup**:  
  - Customizable layout dimensions  
  - Adjustable barrier density  
  - Flexible start/finish positioning  

- **Enhanced ACO Engine**:  
  - Colony of pathfinding agents  
  - Evolving scent trail mechanism  
  - Real-time parameter optimization  
  - Smart dead-end recovery  

- **Algorithm Fusion**:  
  - Hybrid ACO + Dijkstra integration  
  - Tunable balance between exploration and certainty  

- **Evolutionary Techniques**:  
  - Path recombination in advanced cycles  
  - Selective inheritance of successful routes  

- **Interactive Display**:  
  - Visual terrain mapping  
  - Animated solution tracing  
  - Live performance metrics  

## System Needs  

- Python 3.8+  
- Color-supported command interface  

## How to Use  

1. Launch the navigator:  
   ```bash  
   python ant_navigator.py  

Sample Output:  

ANT COLONY NAVIGATOR CONFIGURATION  
══════════════════════════════════  
Set parameters or accept defaults  

 • Layout: 7x8 grid with 11 barriers (20%)  
 • Origin: (1,0), Destination: (5,7)  
 • Agents: 10, Cycles: 20  
 • Hybrid Ratio: 0.5, Max Retreats: 5  

OPTIMAL PATH DISCOVERED  
Solution length: 11 steps  
```bash  
  0  1  2  3  4  5  6  7  
━━━━━━━━━━━━━━━━━━━━━━━━  
0|   |   |   |   |   |   |   |   |  
1| S | > |   |   | █ |   |   |   |  
2| > |   | █ |   |   |   | █ |   |  
3| > |   |   | █ |   |   |   |   |  
4| > | █ |   |   |   | █ |   |   |  
5| > | > | > | > | > | > | > | G |  
6|   |   |   |   | █ |   |   |   |  

Usage Rights  
This solution is publicly available under open-source guidelines.  

Important Notes  
 • Recommended: Use terminals with full color support  
 • Larger environments may need increased cycles/agents  
 • The hybrid method enhances basic ACO performance  
 • Parameter tuning dramatically impacts results
