# AIChatEnhancer

**AIChatEnhancer** is an advanced tool that enhances chatbot functionality by allowing the integration of custom Node-based functions and tools into the conversation model. It allows developers to add more personalized capabilities to the chat model by utilizing external functions that can be called during the conversation.

## Features

- Integrates custom functions into chatbot interactions.
- Supports tool calls and allows models to use functions as part of the conversation flow.
- Flexible configuration with the ability to set up the system prompt, tools, and other model parameters.
- Compatible with models like Llama3.1, Mistral Nemo, and more that support tool-based interaction.
- Easily extendable with additional tools or modifications.
- Example tools for illustration and immediate use.
- Supports model responses with or without system prompt updates.

## Installation

To integrate **AIChatEnhancer** into your Godot project, follow these steps:

1. Clone this repository or download the `ai_chat_enhancer.gd` script to your project.
2. Add the script as a Node or attach it to your desired Node in the scene.
3. Configure the `target_node`, `tools`, and other parameters to match your specific needs.
4. Customize the `tool_examples` for the tools you wish to integrate into the model.

## Usage

To use **AIChatEnhancer**, create a new instance of the script and assign the target Node on which the model should call functions. You can then provide a list of tools that the model can call during the conversation.

### Example Usage:

```gd
# Inside your main script

var chat_enhancer = AIChatEnhancer.new()
chat_enhancer.target_node = your_target_node  # Node where functions are executed
chat_enhancer.tools = your_tools  # List of tools that the model can call
```

You can add tool examples to help the model understand how to interact with these tools.

## Configuration

- **`target_node`**: The Node that will execute the functions that the model calls during the conversation.
- **`tools`**: An array of `ChatTool` instances, each representing a function the model can use.
- **`built_in_tool_support`**: If set to `true`, the model will process tool calls as built-in capabilities.
- **`tool_examples`**: A list of example interactions that can help train the model on how to use the tools.

## Contributing

Feel free to fork this repository, submit issues, and create pull requests to contribute to the project. Contributions are welcome for bug fixes, new features, and improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project leverages Godot's powerful scripting capabilities and integrates AI-based tool calling.
- Inspired by other advanced chatbot systems that integrate function calling and tool utilization.

## Contact

If you have any questions or suggestions, feel free to reach out or open an issue on GitHub.

---

**AIChatEnhancer** is a tool designed to give your chatbot the power to extend its functionality beyond basic conversation, enabling more advanced use cases and seamless interaction with your custom tools and systems.
