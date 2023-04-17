Redux Road (Codecademy project)

In this project I will try to build an adventure game using reducers, state, and actions.
The state will represent, well, the state of the game. It contains the player’s inventory, distance travelled, and time on the road.
Each event in the game is represented as an action. Players can gather supplies, travel,
and–if they play risky–sometimes tip over the wagon carrying their supplies.


Initial State and Reducer
1. First, define the starting point of our game. The player begins on day 0 at kilometer 0 with 100 units of supplies.
2. Define an empty reducer that will manage the state of the game. You can give it any name you prefer.
3. Add a switch statement to your reducer. The default case should return the state.
4. A player may gather supplies, which takes them a day and doesn’t cover any distance.
5. A player may travel for any number of days, which costs 20 supplies for each day but adds 10 kilometers each day.
6. If a player drives off-road or across deep rivers, the wagon may tip! You’ll need to spend some supplies and a day to fix it.
7. Let’s try our game out.
8. Our first day will be dedicated to travel. Call the reducer with the wagon state and an action with type: 'travel' and payload: 1.
9. On the second day, we stop to gather supplies.Call the reducer with the new wagon state and an action with type: 'gather' and no payload.
10. On the third day, we try to ford a rushing river…and our wagon tips over, spilling some supplies.Call the reducer with the new wagon state and an action with type: 'tippedWagon'.
11. On the following day, we set out for a long 3 days of travel. Call the reducer with the new wagon state and an action with type: 'travel' and a payload: 3.
12. Currently, the player can continue traveling even if their supplies are negative! Fix this in the 'travel' case.If there are not sufficient supplies to travel the given number of days, return the current state.
13. Extra practice
 (a) Add a cash property, beginning with 200 for the initial state 
 (b) Add a 'sell' case: Players can give away 20 supplies to gain 5 cash 
 (c) Add a 'buy' case: Players can gain 25 supplies at the cost of 15 cash 
 (d) Add a 'theft' case: Outlaws steal half of the player’s cash
