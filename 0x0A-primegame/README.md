# Prime Game

Maria and Ben are playing a game in which they take turns selecting prime numbers from a set of consecutive integers starting from 1 up to a given number, `n`. The player who cannot make a move loses the game. They play multiple rounds of the game, with different values of `n` for each round.

Assuming Maria always goes first and both players play optimally, the task is to determine who wins each game. 

## Function Signature
```python
def isWinner(x, nums):
    pass
```

## Parameters
- `x`: The number of rounds played.
- `nums`: An array containing `n` for each round.

## Returns
- The name of the player who won the most rounds.
- If the winner cannot be determined, return `None`.

## Constraints
- `n` and `x` will not be larger than 10,000.
- No external packages are allowed.

## Example
```python
x = 3
nums = [4, 5, 1]

isWinner(x, nums)
```
### Output
Ben has the most wins

### Explanation
- **First round:**
  - Maria picks 2 and removes 2, 4, leaving 1, 3.
  - Ben picks 3 and removes 3, leaving 1.
  - Ben wins because there are no prime numbers left for Maria to choose.
  
- **Second round:**
  - Maria picks 2 and removes 2, 4, leaving 1, 3, 5.
  - Ben picks 3 and removes 3, leaving 1, 5.
  - Maria picks 5 and removes 5, leaving 1.
  - Maria wins because there are no prime numbers left for Ben to choose.
  
- **Third round:**
  - Ben wins because there are no prime numbers for Maria to choose.

Therefore, Ben has the most wins overall.

---
This game is played with different rounds, each with its own set of rules. The winner of each round is determined by the strategic choices made by both players.