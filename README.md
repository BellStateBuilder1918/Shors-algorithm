
# Shor's Algorithm Implementation


## Overview
Shor's Algorithm is a groundbreaking quantum algorithm that efficiently factors large composite numbers, a task that is computationally expensive for classical computers. The algorithm has significant implications for cryptography, particularly for RSA encryption.

## Features
- **Quantum Circuit Construction**: The implementation includes a quantum Fourier transform (QFT) and controlled unitary gates.
- **Quantum Simulation**: Uses `Cirq`'s simulator to emulate quantum behavior.
- **Randomized Inputs**: Option to randomly select a base for testing the algorithm.

## Requirements
This implementation requires the following dependencies:

- Python 3.x
- `cirq`
- `numpy`

To install the dependencies, run:

```bash
pip install cirq numpy
```

3. Enter a composite number (N) when prompted. Optionally, provide a base (a) or leave it blank to use a random value.

## Example
Input:
```
Enter composite number N: 15
Enter base a (leave blank for random selection): 2
```
Output:
```
Randomly chosen a: 2
Quantum order measurements: [[0 1 0]
 [1 0 1] ...]
Factors of 15: (3, 5)
```

## Limitations
- The algorithm assumes the input is a composite number.
- The implementation may not always succeed due to randomization; re-running with different inputs may help.


## License
This project is licensed under the MIT License. See the `LICENSE` file for details.


