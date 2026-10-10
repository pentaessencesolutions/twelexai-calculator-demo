# Calculator Application – Implementation Instructions

## Objective

Build a secure, responsive calculator web application using vanilla HTML, CSS, and JavaScript.

## Functional requirements

The calculator must support:

- Addition
- Subtraction
- Multiplication
- Division
- Decimal numbers
- Negative numbers
- Percentage calculation
- Clear/reset
- Delete last character
- Keyboard input
- Enter key to calculate
- Escape key to clear
- Divide-by-zero error handling
- Calculation history showing the five most recent calculations

## User interface

- Display the current expression and result.
- Use a responsive layout suitable for desktop and mobile.
- Provide visible hover and keyboard-focus states.
- Use accessible button labels.
- Ensure sufficient color contrast.
- Show readable validation and calculation errors.

## Technical requirements

- Use HTML5, CSS3, and JavaScript ES modules.
- Do not use `eval`, `Function`, or similar dynamic code execution.
- Do not use inline JavaScript event handlers.
- Keep calculation logic separate from DOM/UI logic.
- Do not require a backend service.
- Avoid third-party runtime dependencies.

## Required structure

Create or update these files:

- `index.html`
- `styles.css`
- `src/app.js`
- `src/calculator.js`
- `tests/calculator.test.js`
- `package.json`
- `README.md`

## Calculation API

`src/calculator.js` should export testable functions for:

- `add`
- `subtract`
- `multiply`
- `divide`
- `percentage`
- Expression or calculator-state processing

Division by zero must return a controlled error and must not produce `Infinity`.

## Tests

Use Node.js's built-in test runner.

Tests must cover:

- Addition
- Subtraction
- Multiplication
- Division
- Decimal calculations
- Negative numbers
- Percentage calculations
- Division by zero
- Invalid input
- Clear/reset behavior

The following command must pass:

    npm test

## Security requirements

- Never use `eval` or the `Function` constructor.
- Never insert untrusted values using `innerHTML`.
- Validate calculator input before processing it.
- Do not add credentials, tokens, or secrets to the repository.
- Do not load executable scripts from third-party CDNs.

## Documentation

Update `README.md` with:

- Application overview
- Features
- Local usage instructions
- Test instructions
- Project structure
- Security decisions

## Definition of done

The task is complete only when:

1. All required
