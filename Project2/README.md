# Digital Design: Coffee Machine Dispenser

## Project Overview

This project involves the design and simulation of a coffee machine dispenser controller. The machine accepts 50 Kr (0.5 TL) and 1 TL coins and dispenses Latte, Turkish coffee, and Cappuccino. 

Key operational properties of the coffee machine:

- Accepts only 50 Kr (0.5 TL) and 1 TL coins.
- Dispenses Latte for 50 Kr, Turkish coffee for 1 TL, and Cappuccino for 2 TL.
- Provides change if extra coins are inserted. E.g., If a customer inserts 1 TL and selects Latte, the machine returns 50 Kr.
- Includes a reset button to abort operations and return all inserted money at any time.
- Only one input can be active at a given time.
- Can dispense a product in one clock cycle.
- The state machine remains in the current state if no inputs are active.

# Report

This project report documents the design and simulation of a coffee machine dispenser controller. The machine takes coins as input and dispenses three different types of coffee (and possibly change coins) as the output. The report explains the individual steps of the design, the state tables, design schematics, strategies, and simulations.

## Design Steps 

### Step 1: Specifications of the Desired Circuit

The coffee machine accepts 50 kuruş and 1 lira coins and dispenses three types of coffee:

- Latte: 50 kuruş
- Turkish Coffee: 1 lira
- Cappuccino: 2 lira

The machine also has a coin return button and can only accept one input at a time. The machine can dispense a product in one clock cycle. If more than 2 lira is inserted, the excess money is automatically returned. If no inputs are active, the state machine stays in the current state.

### Step 2: State Diagram

The state diagram represents all possible states and the conditions for transitioning from one state to the next. The detailed state diagram is available in the project report.

### Step 3: State Table

The state table, derived from the state diagram, captures the behavior of the system in tabular form.

### Step 4: Synthesis Using D Flip-Flops

The design is implemented using D flip-flops. The next-state logic expressions were derived to develop the input logic circuit. The logic expressions for the output logic circuit were also derived. More information is available in the project report.

### Step 5: Implementation & Simulation

The design was implemented with D flip-flops, AND gates, OR gates, and inverters. The simulation of the single D flip-flop and the total project with all inputs and outputs is included in the report.


