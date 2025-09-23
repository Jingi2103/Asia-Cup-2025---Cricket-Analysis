**Asia Cup 2025** – Live Title Probability Tracker
Overview

This repository contains a Python-based simulation to track the probability of each Super-4 team (India, Pakistan, Sri Lanka, Bangladesh) winning the Asia Cup 2025.

The simulation considers:

Current wins and losses

Net Run Rate (NRR)

Toss impact (who wins the toss)

Chasing vs defending advantage

Monte Carlo simulations are used to estimate title-winning probabilities and generate charts showing probability trends over time.

Features

Simulate remaining Super-4 matches and finals.

Dynamic line charts showing probability trends for all teams.

Tables displaying final probabilities for each team.

Incorporates toss and strategy factors (chase/defend advantages).

Easy to update after each match for live analytics.

Getting Started
Prerequisites

Python 3.x

Libraries: numpy, matplotlib

Install dependencies:

pip install numpy matplotlib

How to Run

Update the teams dictionary with current wins, matches, NRR, chase/defend advantage.

Update the remaining_matches_master list with matches yet to be played.

Run the simulation script:

python asia_cup_simulation.py


The script will output:

Final probabilities table

Probability trend chart

Example Teams Dictionary
teams = {
    "India":      {"wins": 4, "matches": 4, "nrr": 0.689, "chase_adv": 1, "defend_adv": 1},
    "Pakistan":   {"wins": 2, "matches": 4, "nrr": -0.689, "chase_adv": 0, "defend_adv": 0.5},
    "SriLanka":   {"wins": 3, "matches": 4, "nrr": -0.121, "chase_adv": 1, "defend_adv": 0},
    "Bangladesh": {"wins": 3, "matches": 4, "nrr": 0.121, "chase_adv": 1, "defend_adv": 0.5},
}

Remaining Matches Example
remaining_matches_master = [
    ("Pakistan", "SriLanka"),
    ("India", "Bangladesh"),
    ("Pakistan", "Bangladesh"),
    ("India", "SriLanka"),
]

Output

Line chart: Shows probability trends for each team over time.

Table: Shows final title probabilities after simulating all remaining matches.

Favorite team & most likely final are highlighted.

Usage Tips

Update the teams stats after every match to see live probability changes.

Charts can be exported as PNG to include in blogs or reports.

Track changes in toss and chase/defend advantage to see their impact on team probability.

License

This project is licensed under the MIT License.
