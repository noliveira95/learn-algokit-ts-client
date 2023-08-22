# Learn Autogenerated AlgoKit TS Client with Calculator App

This project is meant to be cloned and used to follow along the [AlgoKit App Client Explained](https://www.youtube.com/watch?v=xl9kekYIHCc) video. With this project, you will learn how to set up your development environment with `algokit bootstrap all`, how to generate a typescript client for contract interaction with `algokit generate` and use the generated client to interact with a calculator smart contract.

## Contents

📂**smart_contract** - _Directory containing files related to the calculator smart contract_ </br>
┃ 📂**artifacts** - _Directory containing autogenerated artifacts_ </br>
┃ 📜**build.py** - _Python script that generates artifacts from the PyTeal/Beaker smart contract_ </br>
┃ 📜**calculator.py** - _Calculator smart contract in PyTeal/Beaker_ </br>
┃ 📜**deploy.ts** - _Deploy/interact script with the contract using the generated ts client_ </br>
┃ 📜**.env** - _Contains localnet env variables_ </br>

## Setup

1. Ensure you have AlgoKit installed and run `algokit bootstrap all` in this directory
2. Go into the `smart_contract` folder by running `cd smart_contract`
3. Generate ts client with `algokit generate client artifacts/ --output artifacts/client.ts`. Learn more about `algokit generate` [here](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/features/generate.md)
4. Ensure you have Docker running and launch Localnet with `algokit localnet start`
5. Run the `deploy.ts` file by running `npm run deploy` in the **smart_contract folder**

## Tools

The following tools are used in this project:

- [Algorand](https://www.algorand.com/) - Layer 1 Blockchain; [Developer portal](https://developer.algorand.org/), [Why Algorand?](https://developer.algorand.org/docs/get-started/basics/why_algorand/)
- [AlgoKit](https://github.com/algorandfoundation/algokit-cli) - One-stop shop tool for developers building on the Algorand network; [docs](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/algokit.md), [intro tutorial](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/tutorials/intro.md)
- [Beaker](https://github.com/algorand-devrel/beaker) - Smart contract development framework for PyTeal; [docs](https://beaker.algo.xyz), [examples](https://github.com/algorand-devrel/beaker/tree/master/examples)
- [PyTEAL](https://github.com/algorand/pyteal) - Python language binding for Algorand smart contracts; [docs](https://pyteal.readthedocs.io/en/stable/)
- [AlgoKit Utils](https://github.com/algorandfoundation/algokit-utils-py) - A set of core Algorand utilities that make it easier to build solutions on Algorand.
- [Poetry](https://python-poetry.org/): Python packaging and dependency management.
