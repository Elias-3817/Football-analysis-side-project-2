# Football Analysis Side Project

## Overview
In modern football, traditional positional roles have evolved significantly. A player may be listed as an attacking midfielder in a starting XI but perform a role entirely different from the classic number 10. Others may start out wide but drift centrally, functioning more like an attacking midfielder. Similarly, fullbacks now operate in diverse roles—acting as third center-backs in buildup, shifting into midfield as inverted fullbacks, or pushing high as auxiliary wingers.

Given these positional fluidities, this project examines Subjective Offensive Midfielders—players whose roles align with attacking midfield responsibilities, regardless of their listed positions. To create this dataset, I manually reviewed heatmaps of multiple players across different teams to determine if they fit this category. Once identified, I analyzed their statistical outputs, with a particular focus on Curtis Jones and other Liverpool midfielders, to assess their strengths and areas of influence.

This repository contains data analyses for evaluating these subjective offensive midfielders in football. The project utilizes various statistical metrics to assess player performance across multiple aspects of the game.

## Project Structure
```
Football-analysis-side-project-2/
│
├── Subjective Offensive Midfielders Data/
│   ├── Code/                # Python scripts for data analysis
│
```

## Technologies Used
- **Python** – For data processing and analysis
- **Pandas** – Data manipulation
- **Matplotlib & Seaborn** – Visualization tools

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/Elias-3817/Football-analysis-side-project-2.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Football-analysis-side-project-2
   ```
3. Run Python scripts (if available) in the `Code` directory to generate or update analyses.

## Findings

### Shot Selection & Frequency
- Curtis Jones is a cautious and selective shooter, primarily taking shots inside the penalty area (average shot distance: 15.2 yards).
- He averages 2 shots per 90 minutes inside the box, likely due to Liverpool's dominance in most matches.
- Alexis Mac Allister has a similar shot profile but takes fewer shots overall due to his deeper positioning.

### Expected Assists (xA) & Creativity
- Curtis Jones has extremely low xA numbers, to the point that he is nearly excluded from the dataset.
- This aligns with his ball-retention-focused playstyle, prioritizing possession over riskier passes.
- Alexis Mac Allister is Liverpool’s most creative midfielder in terms of chance creation.
- Mikkel Damsgaard, Youri Tielemans, and Bruno Guimarães stand out as elite creative midfielders, playing an integral role in their teams' attacking output.

### Goals & Assists Contribution
- Liverpool’s attacking midfielders have room for improvement in terms of goal contributions.
- Mikkel Damsgaard is once again a standout playmaker.
- Cole Palmer receives praise, but his high numbers are not surprising.

### Ground Duels Won
- Ryan Gravenberch is Liverpool’s best duel winner, performing well in physical contests.
- Alexis Mac Allister also deserves credit for engaging in many duels and maintaining a win rate above 50%.
- Dominik Szoboszlai has been disappointing in duel-winning ability.
- Bruno Guimarães, Youri Tielemans, and Carlos Baleba stand out as dominant midfielders in duels.

### Long Pass Accuracy
- Curtis Jones struggles in this area, attempting fewer long passes and completing them at a lower percentage.
- Moisés Caicedo appears to be the best midfielder for long passing.

### On-Off Impact (Interpretation with Caution)
(On-off stats reflect team performance with vs. without a player on the field, but they can be skewed by strength of opposition.)
- Bernardo Silva has the worst on-off difference, suggesting his team struggles when he plays.
- Youri Tielemans and Bruno Guimarães appear crucial to their teams, as their absence negatively impacts results.

### Passing Completion & Progressive Passing
- Curtis Jones has the highest pass completion rate in the dataset but attempts the fewest progressive passes per game.
- Deeper midfielders tend to have higher progressive passing distance, which aligns with expectations.
- Youri Tielemans, Bruno Guimarães, Moisés Caicedo, and Mateo Kovačić stand out, with Kovačić excelling in both progressive distance and accuracy.

### Press Resistance Index & Take-Ons
(Since no standardized press resistance data exists, I created an index based on key attributes:)

#### Press Resistance Index Formula:
**Positive Factors (higher is better):**
- Take-ons attempted per 90 (20% weight)
- Successful take-on percentage (45% weight)
- Pass completion percentage (20% weight)
- Progressive carries per 90 (20% weight)

**Negative Factors (lower is better):**
- Tackled during take-ons percentage (45% weight)
- Miscontrols per 90 (35% weight)
- Dispossessed per 90 (40% weight)

**Findings:**
- Ryan Gravenberch and Curtis Jones are Liverpool’s most press-resistant midfielders.
- Mohammed Kudus and Tyler Dibling also rank very highly.
- The index is not perfect, but it provides useful insights.

### Progressive Actions (Passes & Carries)
- Curtis Jones struggles in progressive passing and carrying, likely due to his cautious playstyle.
- Dejan Kulusevski, Bruno Fernandes, Bruno Guimarães, and Youri Tielemans excel in progressive actions.

### Shot & Goal Creation Actions per 90
- Dominik Szoboszlai thrives in creating chances and scoring opportunities.
- Kevin De Bruyne, even past his peak, remains elite.
- James Tavernier, Amad Diallo, James Maddison, and Mikkel Damsgaard all stand out.

### Tackles Won & Interceptions per 90
- Ryan Gravenberch leads Liverpool in interceptions per game.
- Alexis Mac Allister ranks 4th in tackles per game.
- Idrissa Gueye, Carlos Baleba, Christian Nørgaard, and Elliot Anderson stand out as top defensive midfielders.
- Curtis Jones was nearly at zero in both metrics, requiring manual addition to the plot.

### Total Duels Won & Duel Win Percentage
(This dataset includes aerial duels, so findings are similar to ground duels and will not be elaborated on.)

## Future Improvements
- Expanding analysis beyond offensive midfielders
- Enhancing dataset with more advanced metrics
- Potential integration of machine learning for deeper insights

## Contributions
Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

## License
This project is licensed under the MIT License.

