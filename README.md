# Baseball Pitcher Performance Analysis

A comprehensive Python-based analytics pipeline for evaluating pitcher performance using pitch-level tracking data. This project generates statistical summaries, visualizations, and comparative analyses to identify pitching strengths, weaknesses, and strategic patterns.

## 📊 Project Overview

This analysis toolkit processes pitch-level tracking data to provide deep insights into pitcher performance, including:
- Strike zone command and location patterns
- Pitch arsenal composition and usage
- Effectiveness metrics (strike%, whiff%, contact%)
- Stuff quality indicators (velocity, spin rate)
- Comprehensive pitcher-level and game-level comparisons

## 🎯 Key Features

### Statistical Analysis
- **Pitcher Performance Summary**: Comprehensive pitcher-level statistics including effectiveness metrics, stuff quality indicators, and arsenal composition
- **Game-Level Comparison**: Aggregated performance metrics comparing overall pitching between games
- **Pitch Type Effectiveness**: Granular breakdown of individual pitch type performance for each pitcher

### Visualizations
- **Strike Zone Heat Maps**: Location density maps showing command patterns for top pitchers
- **Pitch Arsenal Breakdown**: Stacked bar charts revealing pitch type distribution and arsenal diversity
- **Effectiveness Metrics Comparison**: Multi-metric comparison charts for identifying elite performers
- **Velocity vs Spin Rate Analysis**: Scatter plots evaluating raw stuff quality across pitchers

## 📁 Project Structure

```
├── Abdalla_Damario_Code.ipynb    # Main analysis notebook
├── README.md                       # Project documentation
└── data/
    └── pitch_data.csv            # Sample pitch-level data
```

## 🔧 Requirements

### Dependencies
```python
pandas
numpy
matplotlib
scipy
```

### Installation
```bash
pip install pandas numpy matplotlib scipy
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib scipy
```

### Usage

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/baseball-pitcher-analysis.git
cd baseball-pitcher-analysis
```

2. **Prepare your data**
   - Place your pitch-level CSV file in the project directory
   - Data should include columns: GamePk, PitcherId, PitchCall, PlateLocSide, PlateLocHeight, RelSpeed, SpinRate, TaggedPitchType

3. **Run the analysis**
   - Open `Abdalla_Damario_Code.ipynb` in Jupyter Notebook or Google Colab
   - Update the file path in the notebook to point to your data file
   - Execute cells sequentially starting with the library imports
   - Each analysis section can be run independently after loading libraries

4. **View outputs**
   - CSV tables: `pitcher_summary_table.csv`, `game_comparison_table.csv`, `pitch_type_effectiveness_detail.csv`
   - PNG visualizations: `pitch_arsenal_breakdown.png`, `strike_zone_heatmaps.png`, `effectiveness_comparison.png`, `velocity_spin_scatter.png`

## 📈 Analysis Components

### 1. Pitcher Performance Summary (Table 2)
Generates comprehensive pitcher-level statistics:
- **Effectiveness metrics**: Strike%, Whiff%, Contact%
- **Stuff quality**: Average/Max velocity, Average spin rate
- **Arsenal composition**: Primary and secondary pitch types with usage percentages

### 2. Pitch Arsenal Visualization (Figure 1)
Creates stacked bar chart showing pitch type distribution for pitchers with 20+ pitches, revealing:
- Arsenal diversity
- Strategic pitch selection differences
- Color-coded pitch type breakdown

### 3. Strike Zone Heat Maps (Figure 2)
Visualizes pitch location patterns for top 2 pitchers from each game:
- Heat map intensity shows pitch concentration
- Strike zone overlay from catcher's perspective
- Reveals command tendencies and targeting strategies

### 4. Effectiveness Metrics Comparison (Figure 3)
Compares four key metrics across all pitchers (20+ pitches):
- **Strike%**: Overall command and strike-throwing ability
- **Whiff%**: Swing-and-miss capability
- **Zone%**: Aggression and attack mentality
- **Chase%**: Deception and ability to induce swings outside zone

### 5. Game-Level Comparison (Table 1)
Aggregates and compares performance between Game 1 and Game 2:
- Workload metrics (total pitches, unique pitchers)
- Effectiveness rates (strike%, ball%, swing%, whiff%, contact%)
- Results-based metrics

### 6. Velocity vs Spin Rate Analysis (Figure 4)
Scatter plot evaluating raw stuff quality:
- Velocity on x-axis, spin rate on y-axis
- Bubble size represents pitch count (workload)
- Identifies elite stuff versus command-based pitchers

### 7. Pitch Type Effectiveness Detail (Table 3)
Granular pitch-by-pitch breakdown showing:
- Individual pitch type performance per pitcher
- Primary weapons versus developmental pitches
- Usage percentages and effectiveness by pitch type

## 📊 Key Metrics Explained

- **Strike%**: Percentage of pitches resulting in strikes (called, swinging, fouls)
- **Whiff%**: Percentage of swings that miss the ball
- **Contact%**: Percentage of swings that make contact
- **Zone%**: Percentage of pitches thrown in the strike zone
- **Chase%**: Percentage of swings on pitches outside the zone

## 🎓 Applications

This analysis framework is valuable for:
- Personal baseball analytics projects and portfolio development
- Understanding pitcher performance evaluation methodologies
- Learning data visualization and statistical analysis techniques
- Exploring relationships between pitch characteristics and outcomes
- Developing insights into modern pitching strategies

## 💡 Project Motivation

This project demonstrates the application of data science techniques to baseball analytics, showcasing skills in:
- Data manipulation and cleaning with pandas
- Statistical analysis and metric calculation
- Data visualization with matplotlib
- Performance evaluation framework design
- Translating complex data into actionable insights

## 📝 Data Requirements

Input CSV should contain the following columns:
- `GamePk`: Game identifier
- `PitcherId`: Unique pitcher identifier
- `PitchCall`: Outcome of the pitch (called_strike, ball, swinging_strike, etc.)
- `PlateLocSide`: Horizontal pitch location
- `PlateLocHeight`: Vertical pitch location
- `RelSpeed`: Pitch velocity
- `SpinRate`: Pitch spin rate (RPM)
- `TaggedPitchType`: Pitch type classification (FF, SL, CU, CH, etc.)

**Note**: Sample data used in this project analyzed 620 pitches across two games from 17 pitchers.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page or submit a pull request.

## 📄 License

This project is available under the MIT License.

## 👤 Author

**Damario Abdalla**

- Portfolio project showcasing baseball analytics capabilities
- Built with Python data science stack (pandas, numpy, matplotlib, scipy)

## 🙏 Acknowledgments

- Inspired by modern baseball analytics methodologies
- Statistical frameworks based on industry-standard performance metrics
