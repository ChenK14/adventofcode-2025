# 🎄 Advent of Code 2025

A JavaScript starter template for [Advent of Code 2025](https://adventofcode.com/2025).

## Getting Started

```bash
git clone https://github.com/ChenK14/adventofcode-2025.git
cd adventofcode-2025
npm install
```

## Project Structure

Each day has its own folder (`day1/`, `day2/`, etc.) with:
- `dayX.js` - Your solution code
- `input.txt` - Your personal puzzle input (get it from adventofcode.com)

## Solving a Puzzle

### 1. Get your input from AOC
- Go to https://adventofcode.com/2025/day/X
- Copy your puzzle input
- Paste it into `dayX/input.txt`

### 2. Write your solution in `dayX/dayX.js`

```javascript
const solvePuzzle1 = (lines, testing) => {
  if (!testing) {
    lines = getLinesFromPath("dayX/input.txt")
  }
  // Your solution here - 'lines' is an array of strings
  return yourAnswer
}
```

### 3. Add tests in `adventofcode.spec.js`

Uncomment the day's test block and add the example from AOC:

```javascript
describe("Day X", () => {
    const testInput = [
      "example line 1",
      "example line 2",
      // paste the example from the puzzle here
    ]
    test("puzzle 1 test", () => {
        expect(solvePuzzle1DayX(testInput, true)).toBe(EXPECTED_EXAMPLE_ANSWER)
    })
    test("puzzle 1 forReal", () => {
        expect(solvePuzzle1DayX(testInput, false)).toBe(YOUR_REAL_ANSWER)
    })
    // same for puzzle 2...
})
```

## Running Tests

```bash
npm test                     # Run all tests
npm test -- --watch          # Watch mode (re-runs on file changes)
npm test -- -t "Day 1"       # Run only Day 1 tests
```

## Tips

- The `testing` parameter tells you if you're running with example input (`true`) or real input (`false`)
- Start by making the example pass, then run with your real input
- Each day has 2 puzzles - Part 2 unlocks after you solve Part 1

Good luck! 🎅

