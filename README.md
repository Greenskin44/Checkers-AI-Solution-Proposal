# Academic Research Portfolio

## Checkers AI Solution Proposal: A Comparative Analysis of Search Algorithms for Strategic Game-Playing

**Author:** Noah Rundell  
**Institution:** Southern New Hampshire University  
**Course:** IT-450 Artificial Intelligence  
**Date:** June 2025  
**Length:** 23 pages

---

## Abstract

This research paper presents a comprehensive comparative analysis of three distinct AI paradigms applied to strategic game-playing in checkers: rule-based inference systems, heuristic search with minimax, and Monte Carlo Tree Search (MCTS). The study demonstrates how hybrid approaches combining symbolic AI with statistical methods achieve superior performance compared to either paradigm alone, with empirical testing showing MCTS achieving a 62% win rate against minimax opponents.

## Research Overview

### Problem Domain

Checkers serves as an ideal benchmark for AI research due to its combination of:
- Adversarial gameplay requiring competitive strategy
- Perfect information (full observability)
- Deterministic state transitions
- Finite game space with well-defined rules

### Key Contributions

1. **Hybrid Architecture Design**: Developed a layered system combining rule-based move generation with statistical search-based selection
2. **Comparative Algorithm Analysis**: Empirically evaluated three AI approaches (greedy heuristic, minimax with alpha-beta pruning, MCTS)
3. **Performance Optimization**: Achieved 99.95% branch reduction through alpha-beta pruning and 62% MCTS win rate
4. **Transferable Framework**: Demonstrated architecture applicable to other perfect information games

## Methodology

### Three AI Paradigms Evaluated

**1. Production Rules (Inference System)**
- Forward-chaining logic for legal move generation
- Implements mandatory capture rule (R3)
- Handles promotion and king movement
- Ensures rule compliance without search

**2. Heuristic Search (Minimax)**
- Constructs game tree to depth 2-4 plies
- Material-based evaluation (pawns=1, kings=3)
- Alpha-beta pruning for efficiency
- Achieves tactical awareness through adversarial reasoning

**3. Monte Carlo Tree Search**
- Statistical alternative requiring no domain-specific evaluation
- Runs 100 random simulations per legal move
- Learns strategy through experience rather than explicit programming
- Naturally discovers tactical concepts

## Key Results

### Performance Comparison

| Method | Response Time | Tactical Depth | Domain Knowledge | Win Rate vs Random |
|--------|--------------|----------------|------------------|-------------------|
| Greedy | <0.1s | None (0-ply) | Hard-coded rules | ~75% |
| Minimax | <1s | Limited (2-ply) | Material evaluation | ~85% |
| MCTS | 1-2s | Adaptive | Statistical learning | **~92%** |

### Significant Findings

- **Alpha-beta pruning reduced node evaluations by ~50%**, enabling deeper search
- **MCTS achieved 62% win rate against minimax**, demonstrating superiority
- **Material-only heuristic proved surprisingly effective** when embedded in search
- **Hybrid approach (rules + statistics) outperformed either paradigm alone**

## Technical Implementation

### Core Technologies
- **Language:** Python
- **Key Libraries:** NumPy (game state representation), time (performance metrics)
- **Algorithms:** Minimax with alpha-beta pruning, Monte Carlo Tree Search, forward-chaining inference

### System Architecture
```
Input State → Inference System (Legal Move Generation) → Search Algorithm (Move Selection) → Output Action
              ↓                                              ↓
         Production Rules                         Minimax or MCTS
         (R1-R5: slides,                     (Statistical evaluation)
          jumps, captures)
```

## Academic Significance

This research demonstrates:
1. **Integration of Multiple AI Paradigms**: Successfully combines symbolic AI (rule-based systems) with statistical methods (MCTS)
2. **Practical Algorithm Comparison**: Provides empirical evidence for performance trade-offs between approaches
3. **Transferable Design Patterns**: Framework applicable to automated planning, robotics, and decision support systems
4. **Pedagogical Value**: Clear progression from greedy algorithms through minimax to advanced MCTS

## Future Directions

Potential enhancements identified:
- Parallel MCTS implementation for deeper search
- Neural evaluation networks trained through self-play
- Domain-aware rollout policies for improved endgame play
- Opening book integration for familiar positions

## How to Access

**Full Paper:** [Rundell_2025_Checkers_AI_Comparative_Analysis.pdf](https://github.com/Greenskin44/Checkers-AI-Solution-Proposal/blob/main/Rundell_Noah_Checkers_AI_Comparative_Analysis.pdf)

### Paper Structure
1. **Introduction** - Problem motivation and AI applicability
2. **Analysis** - AI area classification and visual game elements
3. **Application** - Heuristic method implementation and evaluation
4. **Method Contrast** - Comparison of inference vs. search approaches
5. **Proposal Defense** - MCTS justification and implementation details
6. **Conclusions** - Results synthesis and transferability discussion
7. **Appendix** - Complete figures and code implementations

## Citation

If referencing this work, please use:

```bibtex
@techreport{rundell2025checkers,
  author = {Rundell, Noah},
  title = {Checkers AI Solution Proposal: A Comparative Analysis of Search Algorithms for Strategic Game-Playing},
  institution = {Southern New Hampshire University},
  year = {2025},
  type = {Course Research Paper},
  number = {IT-450}
}
```

## References

Key sources cited in this research:
- Browne et al. (2012) - *A Survey of Monte Carlo Tree Search Methods*
- Knuth & Moore (1975) - *An Analysis of Alpha-Beta Pruning*
- Lucci & Kopec (2015) - *Artificial Intelligence in the 21st Century*

## Contact

**Noah Rundell**  
- LinkedIn: [linkedin.com/in/noah-rundell](https://linkedin.com/in/noah-rundell)
- GitHub: [@Greenskin44](https://github.com/Greenskin44)

---

## Keywords

Artificial Intelligence, Game Playing, Checkers, Minimax, Alpha-Beta Pruning, Monte Carlo Tree Search, Production Rules, Heuristic Search, Inference Systems, Search Algorithms, Adversarial Search, Game Theory

---

*This research was completed as part of the IT-450 Artificial Intelligence course at Southern New Hampshire University under the instruction of Professor Huang.*
