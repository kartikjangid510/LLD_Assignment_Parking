# Design a Pen

This repository contains the design and implementation of a `Pen` with the following required functionalities:

- `start()`
- `write(text)`
- `close()`
- `refill(amount)`

## Assignment Submission

Submit the public GitHub repository link that includes:

- The class diagram for the `Pen` design
- The source code implementation of the `Pen`

## Project Structure

Recommended structure:

```text
.
├── diagrams/
│   └── pen-class-diagram.png
├── src/
│   └── pen.py
└── Readme.md
```

You can adjust file names and language as needed, but make sure both the diagram and implementation are present.

## Pen Design (Class Diagram)

Add your class diagram to `diagrams/` and reference it here:

![Pen Class Diagram](diagrams/pen-class-diagram.png)

Suggested class attributes and behaviors:

- Attributes:
	- `inkLevel`
	- `isOpen`
	- `maxInkCapacity`
- Methods:
	- `start()`
	- `write(text)`
	- `close()`
	- `refill(amount)`

## Functional Requirements

### 1. `start()`

- Opens the pen for writing.
- Should prevent duplicate open operations if already started.

### 2. `write(text)`

- Writes provided text when the pen is started and has ink.
- Consumes ink based on text length (or your chosen logic).
- Should handle cases where ink is insufficient.

### 3. `close()`

- Closes the pen after writing.
- Should prevent duplicate close operations if already closed.

### 4. `refill(amount)`

- Adds ink to the pen.
- Must not exceed maximum ink capacity.
- Should validate invalid refill values (for example, zero or negative amounts).

## Example Behavior

```text
start() -> Pen is now open.
write("Hello") -> Writes text, ink reduced.
close() -> Pen is now closed.
refill(10) -> Ink increased.
```

## How to Run

Document the language-specific steps for your implementation.

Example (Python):

```bash
python src/pen.py
```

## Notes

- Keep the implementation clean and object-oriented.
- Include meaningful validations and error handling.
- Keep class diagram and source code in sync.

