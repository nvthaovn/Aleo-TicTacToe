<!-- # ⭕ Tic-Tac-Toe -->
# Simple Tic-Tac-Toe Game demo

This is A simple game of Tic-Tac-Toe game in Leo for demo purposes only.

⭕ ❕ ⭕ ❕ ❌

➖ ➕ ➖ ➕ ➖

⭕ ❕ ⁣❌ ❕ ⭕

➖ ➕ ➖ ➕ ➖

❌ ❕ ❌ ❕ ⭕

## Requirment 
leo 1.10.0 - https://developer.aleo.org/getting_started/#13-install-leo
Ubuntu 22.04 (tested)

## Install 

```
git clone https://github.com/nvthaovn/Aleo-TicTacToe.git
cd Aleo-TicTacToe
cp .env.sample .env
```

## Config
edit .env file to config your Aleo private key.

## Running the Program

Leo provides users with a command line interface for compiling and running Leo programs.
Users may either specify input values via the command line or provide an input file in `inputs/`.

### Providing inputs via the command line.
1. Run 
```bash
leo run <function_name> <input_1> <input_2> ...
```
See `./run.sh` for an example.


### Using an input file.
1. Modify `inputs/tictactoe.in` with the desired inputs.
2. Run
```bash
leo run <function_name>
```

## Executing the Program
```bash
leo execute <function_name> <input_1> <input_2> ...
```

## Playing the Game

### 1. Create a new game board
```bash
leo run new
```
|   |   |   |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |

### 2. Player 1 makes a move
```bash
leo run make_move 1u8 1u8 1u8 "{ r1: { c1: 0u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
```
|   |   |   |
|---|---|---|
| 1 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |

### 3. Player 2 makes a move
```bash
leo run make_move 2u8 2u8 2u8 "{ r1: { c1: 1u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
```
|   |   |   |
|---|---|---|
| 1 | 0 | 0 |
| 0 | 2 | 0 |
| 0 | 0 | 0 |


## Lience 
https://github.com/AleoHQ/workshop/tree/master/tictactoe