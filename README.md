**Circom Circuit Readme**

This repository contains a Circom 2.0.0 implementation of a simple digital circuit. The circuit includes components for AND, NOT, and OR gates, and a main template that combines these gates to build a more complex logic circuit. This circuit can be used as a basic building block for more sophisticated logic designs.

### Requirements

To use this circuit, you need the following software installed on your system:

- Circom 2.0.0

### Installation and Usage

1. Clone the repository to your local machine:

```
git clone <repository_url>
cd <repository_name>
``

2. Compile the circuit using Circom:

```
npx hardhat circom
```

3. Generate the proof of circuit's constraints using Circom:

```
npx hardhat run scripts/deploy.ts --network mumbai
```

### Circuit Description

The circuit implements a basic logical operation: `(a AND b) OR (NOT b)`, where `a`, `b`, `x`, `y`, and `q` are the input and output signals. The circuit is constructed using three components:

- **AND Gate**: Takes two input signals, `a` and `b`, and outputs the logical AND of these inputs.

- **NOT Gate**: Takes one input signal, `in`, and outputs the logical NOT of this input.

- **OR Gate**: Takes two input signals, `a` and `b`, and outputs the logical OR of these inputs.

The `CircomCircuit` template combines these gates to create a more complex logic circuit.

### Input and Output

- `a` and `b` are input signals, and their values can be set before running the circuit.

- `q` is the output signal, representing the result of the logical operation `(a AND b) OR (NOT b)`.

### Contributing

If you find any issues with the circuit or have suggestions for improvements, feel free to open an issue or submit a pull request. Contributions are welcome!

### License

This project is licensed under the [MIT License](LICENSE).

---
