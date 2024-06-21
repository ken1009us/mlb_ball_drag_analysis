# MLB Ball Drag Analysis

## Overview

This repository contains an analysis of the drag coefficient of baseballs used in Major League Baseball (MLB) over the past five seasons. The purpose of this analysis is to determine whether the properties of the ball have changed, contributing to higher home run rates as some have claimed.

The prompt suggested that many believe the surge in home runs is attributable to a change in the ball's drag coefficient. A lower drag coefficient would enable the ball to travel further through the air, resulting in more home runs.

## Idea

1. Home Run Rates Analysis:

When we look at home run rates over time, we're essentially asking, "Are batters hitting more dingers now than they used to?" If we see an upward trend, it could support the "juiced ball" theory, but it's not definitive proof.

Here's why: Imagine you're coaching a team, and suddenly your players are hitting more home runs without changing their swing or strength training. You'd probably wonder, "What's changed?" One possibility is that the ball itself has changed. A "juiced" ball typically travels farther for the same hit, which could turn some deep fly balls into home runs.

However, we'd also consider other factors:

- Are batters changing their approach, maybe trying to hit more fly balls?
- Have there been changes in pitcher strategies or the types of pitches thrown?
- Are there any changes in ballpark dimensions or environmental factors?

2. Hit Distances Over Time:

This analysis is like asking, "Are our well-hit balls traveling farther than they used to?" If we see an increase in hit distances over the years, it could suggest that something about the ball has changed.

- Outfielders having to play deeper
- More balls reaching the warning track or going over the fence
- Longer doubles and triples

But again, we need to consider other factors:

- Have batters gotten stronger or improved their swing mechanics?
- Are there changes in weather patterns or air density at ballparks?


3. Exit Velocity vs. Hit Distance Relationship:

This is crucial for understanding if the ball's behavior has changed. We're asking, "For the same swing and contact, is the ball traveling farther?"

Imagine two identical hits from different seasons:

- In 2016, a batter hits a ball at 100 mph exit velocity, and it travels 390 feet.
- In 2020, a batter hits a ball at 100 mph, but it travels 405 feet.

If we consistently see this pattern, it suggests the ball might have less drag, allowing it to travel farther for the same initial velocity.

4. Spin Rates Analysis:

Spin rate affects how a ball moves through the air. For a coach, understanding spin rate is like knowing the "movement" on a pitch or the "carry" on a fly ball.

If we see changes in spin rates over time, it could indicate:

- Changes in the ball's surface texture
- Alterations in the ball's core or composition

This could affect both pitching (more or less movement on pitches) and hitting (how the ball behaves off the bat).

5. Statistical Test on Hit Distances:

This test helps us determine if the changes we're seeing are statistically significant or just random variation. It's like asking, "Are these changes real, or are we just seeing things?"

For a coach, it's the difference between making strategic adjustments based on a true trend versus overreacting to a short-term fluctuation.

6. Speed Loss from Release to Plate:

This analysis looks at how much speed a pitch loses on its way to the plate. If the ball has less drag, we'd expect to see less speed loss over time.

- Pitches seeming to have more "life" at the plate
- Fastballs maintaining velocity better
- Changes in how breaking pitches move

7. Correlation Heatmap:

This gives us a big-picture view of how different factors relate to each other. For a coach, it's like understanding the interconnected aspects of the game.

For example, if we see a strong correlation between exit velocity and distance, but this correlation changes over time, it might suggest changes in the ball's properties.

## Data Description

The dataset includes batted ball data from the past five seasons with the following fields:

1. `year`
2. `month`
3. `pitcher_throws` ('L' for left-handed pitcher, 'R' for right-handed pitcher)
4. `bat_side` ('L' for left-handed batter, 'R' for right-handed batter)
5. `pitch_type` ('FF' for four-seam fastball, 'FT' for two-seam fastball)
6. `release_speed` (velocity of the pitch at 50' in mph)
7. `plate_speed` (velocity of the pitch as it crosses home plate in mph)
8. `hit_exit_speed` (velocity of the batted ball upon contact in mph)
9. `hit_spinrate` (rate of rotation of the ball upon contact in rpm)
10. `hit_vertical_angle` (launch angle in degrees)
11. `hit_bearing` (direction from home plate to the initial landing position in degrees)
12. `hit_distance` (distance from home plate to the initial landing position in feet)
13. `event_result` (category of batted ball event outcome)

## Instructions

1. Clone the repository:

```bash
$ git clone https://github.com/your-username/MLB_Ball_Drag_Analysis.git
```

2. Navigate to the project directory:

```bash
$ cd mlb_ball_drag_analysis
```

3. Install required packages:

```bash
$ pip install -r requirements.txt
```
