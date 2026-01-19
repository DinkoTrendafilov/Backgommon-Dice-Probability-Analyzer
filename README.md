# 🎲 Backgammon Dice Probability Analyzer

**Complete statistical analysis of dice sums for Backgammon strategy optimization**

## 📊 Overview

This Python tool performs comprehensive probability analysis of two-dice sums in Backgammon. It calculates exact probabilities, frequencies, and statistical metrics for all possible outcomes when rolling two standard six-sided dice.

## ✨ Features

- **Exact Probability Calculation**: Computes precise probabilities for sums 2 through 12
- **Statistical Analysis**: Mean, median, variance, standard deviation, and mode
- **Cumulative Distribution**: Running probability totals for strategic decision-making
- **Visualization**: Clean bar chart showing frequency distribution
- **Practical Odds**: "1 in X rolls" format for easy game application

## 📈 Key Insights for Backgammon

| Sum | Probability | 1 in X rolls | Strategic Importance |
|-----|-------------|--------------|----------------------|
| 7   | 16.67% | 6.0 | **Most common** - optimal opening moves |
| 6/8 | 13.89% | 7.2 | High priority moves |
| 5/9 | 11.11% | 9.0 | Good blocking opportunities |
| 4/10| 8.33%  | 12.0 | Defensive positions |
| 3/11| 5.56%  | 18.0 | Less common moves |
| 2/12| 2.78%  | 36.0 | Rare - special strategies |

## 🚀 Quick Start

```bash
# Clone repository
git clone https://github.com/DinkoTrendafilov/backgammon-dice-probability.git
cd backgammon-dice-probability

# Install requirements
pip install numpy matplotlib

# Run analysis
python backgammon_dice_analyzer.py


----------------------------------------------------------------------------------------------------------------
Sum: 2  --- Count: 1   | Probability: 2.78%   | Cumulative: 2.78%  | 1 From 36.0 rolls
Sum: 3  --- Count: 2   | Probability: 5.56%   | Cumulative: 8.33%  | 1 From 18.0 rolls
...
Sum: 12 --- Count: 1   | Probability: 2.78%   | Cumulative: 100.00% | 1 From 36.0 rolls
----------------------------------------------------------------------------------------------------------------
STATISTICAL SUMMARY:
Mean: 7.00
Median: 7.00
Variance: 5.83
Standard Deviation: 2.42
Most Common Sum(s): 7
----------------------------------------------------------------------------------------------------------------


📈 Visualization

The tool generates a clean bar chart showing:

    Frequency of each dice sum (2-12)

    Clear labels and grid for easy reading

    Professional styling suitable for presentations


🎯 Strategic Applications
For Backgammon Players:

    Opening Strategy: 7 is most common (16.67%) - plan accordingly

    Risk Assessment: 58.33% chance of rolling 7 or less

    Defensive Planning: 91.67% chance opponent rolls 10 or less

    Doubling Cube: Make mathematically informed doubling decisions

For Game Developers:

    Exact probabilities for game balancing

    Statistical foundation for AI opponents

    Reference data for probability-based games

🧮 Mathematical Foundation

    Total Combinations: 36 (6 × 6)

    Probability Formula: P(sum) = favorable outcomes / 36

    Distribution: Symmetric around mean (7.0)

    Perfect Balance: Mean = Median = Mode = 7


🔧 Requirements

    Python 3.8+

    NumPy

    Matplotlib

Install with:
bash

pip install -r requirements.txt

📝 Usage Examples
Basic Analysis:
python


Get Specific Probabilities:
python

# Get probability of rolling exactly 6
prob_6 = analyzer.get_probability(6)  # Returns 0.1389

# Get probability of rolling 7 or higher
prob_7_plus = analyzer.get_cumulative_probability(7)  # Returns 0.5833

🎲 Practical Backgammon Tips

    Opening Moves: With 7 being most common (1 in 6 rolls), prioritize moves that use 7 pips

    Blocking Strategy: Since 6 and 8 are next most common (1 in 7.2 rolls), secure these points early

    Risk Management: Only 8.33% chance of rolling 11 or 12 - don't rely on these for key plays

    Doubling Decisions: Use cumulative probabilities to assess opponent's likely rolls

📚 Statistical Reference
Metric	Value	Interpretation
Mean	7.00	Average roll over many games
Standard Deviation	2.42	Typical variation from mean
68% Range	4.58 - 9.42	Most rolls fall in this range
95% Range	2.16 - 11.84	Nearly all rolls fall here


🤝 Contributing

Contributions welcome! Please feel free to:

    Add more advanced statistical analyses

    Create visualizations for specific strategies

    Implement Monte Carlo simulations

    Add unit tests

📄 License

MIT License - see LICENSE file for details.
👤 Author

Dinko Trendafilov

    GitHub: @DinkoTrendafilov

    LinkedIn: Dinko Trendafilov

    Email: dinkino79@gmail.com

🌟 Star History

If you find this useful, please consider giving it a star on GitHub!
📊 Related Projects

    Bridge Probability Calculator - Similar analysis for contract bridge

    Game Theory Toolkit - Mathematical tools for game analysis

"In Backgammon, as in life, understanding probabilities is the key to better decisions."
