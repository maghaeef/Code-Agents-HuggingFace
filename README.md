# Code Agents HuggingFace

A framework for creating and deploying code agents powered by Hugging Face models.

## Overview

Code Agents HuggingFace is a project that leverages the power of large language models from Hugging Face to create autonomous coding agents. These agents can help with code generation, debugging, refactoring, and other programming tasks through natural language interaction.

## Features

- **Natural Language Code Generation**: Convert natural language descriptions into functional code
- **Multi-language Support**: Works with various programming languages including Python, JavaScript, Java, and more
- **Customizable Agents**: Create specialized agents for specific programming tasks
- **Easy Integration**: Integrate with existing development workflows and tools
- **Local or Cloud Deployment**: Run models locally or leverage Hugging Face's Inference API

## Installation

```bash
# Clone the repository
git clone https://github.com/maghaeef/Code-Agents-HuggingFace.git
cd Code-Agents-HuggingFace

# Install dependencies
pip install -r requirements.txt
```

## Quick Start

```python
from code_agents import CodeAgent

# Initialize a code agent with a preferred model
agent = CodeAgent(model="codegemma-7b")

# Generate code from a description
result = agent.generate("Create a function that calculates the Fibonacci sequence up to n terms")
print(result.code)

# Explain existing code
explanation = agent.explain("def quick_sort(arr): ...")
print(explanation)
```

## Configuration

Configure your agents by creating a `config.yaml` file in your project directory:

```yaml
model: "codegemma-7b"  # Default model to use
max_tokens: 2048       # Maximum output tokens
temperature: 0.2       # Lower for more deterministic outputs
api_key: "your_key"    # For cloud-based inference
```

## Models

The framework supports various code-specialized models from Hugging Face:

- CodeGemma models
- CodeLlama models
- StarCoder models
- DeepSeek Coder models
- WizardCoder models

## Examples

Check the `examples/` directory for sample applications:

- Code generation assistants
- Automated code review
- Test case generation
- Documentation generation
- Code explanation and teaching

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Hugging Face](https://huggingface.co/) for their amazing models and infrastructure
- All contributors who have helped shape this project

## Contact

- GitHub: [@maghaeef](https://github.com/maghaeef)
- Project Link: [https://github.com/maghaeef/Code-Agents-HuggingFace](https://github.com/maghaeef/Code-Agents-HuggingFace)