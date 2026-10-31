# Head-to-Head Simulator

An interactive browser simulator for testing how a 100-soldier plan performs across five castles. The project is a single HTML file with no build step or runtime dependencies.

## Run it

Open [`Castle battle simulator.html`](./Castle%20battle%20simulator.html) in a modern browser.

The page uses Google Fonts when online, but the simulator itself runs entirely in the browser. No server is required.

## Game modes

Use the **Game** selector to switch between:

### Head to head (Game 1)

- Play against 1–9 generated opponents.
- Each opponent is faced separately.
- At each castle, the player who assigns more soldiers wins that castle's points.
- A tie splits the points.
- Castle values are 1, 2, 3, 4, and 5, for a maximum of 15 points per battle.
- Your result is the average castle points across the selected battles.

### Four-way battle (Game 2)

- Play 1–10 generated groups.
- Each group contains you and three generated opponents.
- At each castle, the player with the most soldiers takes its points; ties split them.
- Players are ranked by total castle points.
- Payouts are 9 points for 1st, 4 for 2nd, 2 for 3rd, and 0 for 4th.
- Tied rankings split the payouts for the tied places.
- Your result is the average payout across the selected groups.

## Using the simulator

1. Assign whole-number soldier counts to the five castles.
2. Make sure the total is exactly 100.
3. Choose a starting plan, number of opponents or groups, and game mode.
4. Click **Play**.
5. Review the individual battles or groups, castle performance, comparison with preset plans, and your overall result.

Included starting plans are:

- My Game 1 plan
- My Game 2 plan
- Proportional
- Even split
- All-in on 4 & 5
- Top three
- All on castle 5
- Custom

## Opponent model

Generated opponents are selected from weighted play styles:

- Proportional
- Even split
- Round numbers
- All-in on 4 & 5
- Top three
- Beat-by-one
- Random
- Two-castle bets

Open **Change the opponent mix** to adjust the style weights and how much each opponent varies from its selected style. Results are randomized each time **Play** is clicked, so repeated runs can differ.

## Project structure

```text
.
├── Castle battle simulator.html
└── README.md
```
