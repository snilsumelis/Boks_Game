# Java Fighter Match Simulation

## Overview
This Java program simulates a match between two fighters. The `Fighter` class represents an individual fighter with attributes such as name, damage, health, weight, and dodge ability. The `Match` class sets up a match between two fighters, considering weight constraints, and simulates the fight with random starting conditions.

## Fighter Class
### Attributes
- **name (String):** The name of the fighter.
- **damage (int):** The damage the fighter can inflict per hit.
- **health (int):** The current health of the fighter.
- **weight (int):** The weight category of the fighter.
- **dodge (double):** The dodge ability of the fighter, represented as a percentage.

### Methods
#### `hit(Fighter foe)`
Simulates a hit by the current fighter on the opponent. Considers the opponent's dodge ability and reduces the opponent's health accordingly.

#### `dodge()`
Determines whether the fighter can dodge an incoming attack based on their dodge ability.

## Match Class
### Attributes
- **f1 (Fighter):** The first fighter in the match.
- **f2 (Fighter):** The second fighter in the match.
- **minWeight (int):** The minimum weight limit for the match.
- **maxWeight (int):** The maximum weight limit for the match.

### Methods
#### `run()`
Runs the match simulation. Checks weight compatibility, randomly selects the starting fighter, and simulates rounds until one of the fighters' health reaches zero.

#### `checkWeight()`
Checks whether the weights of both fighters are within the specified limits for the match.

#### `isWin()`
Checks if one of the fighters has won the match by reducing the opponent's health to zero.

#### `printScore()`
Prints the remaining health of both fighters after each round.

## Usage
1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/snilsumelis/Boks_Game
    ```

2. Navigate to the project directory:
    ```bash
    cd your-repository
    ```

3. Open the project in your preferred Java IDE.

4. Run the `Main` class in the `src` directory to create instances of the `Fighter` and `Match` classes and simulate the fight.

5. Customize fighter information or match constraints by modifying the parameters in the `main` method of the `Main` class.

## Contribution
Feel free to contribute by opening issues or creating pull requests. Contributions are always welcome!

