# Privacy-Preserving Distributed Machine Learning Platform

A scalable and secure platform for collaborative machine learning with privacy guarantees.

## Features

- **Distributed Training**: Train models across multiple participants without data sharing
- **Privacy Protection**: Uses multiple cryptographic techniques (SMPC, HE, DP, ZKP)
- **Scalability**: Designed to handle large numbers of participants and datasets
- **Fault Tolerance**: Continues operation when participants leave or fail
- **Security**: Protection against model poisoning and inference attacks
- **Model Support**: Compatible with linear regression, logistic regression and neural networks
- **Efficiency**: Optimized for reduced communication and computation overhead

## Architecture

- **Client**: Participant nodes that own private data
- **Server**: Orchestrates the training process (without accessing raw data)
- **Crypto**: Cryptographic primitives for privacy-preserving operations
- **Protocols**: Communication protocols for secure multi-party computation
- **Models**: Implementations of various ML models with privacy features
- **Utils**: Utility functions and tools

## Setup

1. Clone this repository
2. Create a virtual environment: `python -m venv venv`
3. Activate the virtual environment: 
   - Windows: `venv\Scripts\activate`
   - Linux/Mac: `source venv/bin/activate`
4. Install requirements: `pip install -r requirements.txt`

## Usage

1. Configure participants in `config.yaml`
2. Start the server: `python -m fedml_privacy.server.main`
3. Start clients: `python -m fedml_privacy.client.main --id CLIENT_ID`

## Security and Privacy Features

- Homomorphic Encryption for secure computations on encrypted data
- Secure Multi-Party Computation for collaborative model training
- Differential Privacy to prevent inference attacks
- Zero-Knowledge Proofs for protocol compliance verification

## Benchmarks

Performance metrics are available in the `benchmarks` directory, measuring:
- Training time
- Communication overhead
- Privacy protection strength
- Model accuracy

## License

MIT 
