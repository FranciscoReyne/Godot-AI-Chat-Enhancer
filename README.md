# GODOT AIChatEnhancer

**AIChatEnhancer** is an advanced tool specifically designed for **Godot Engine** that extends the capabilities of local **Ollama**-based chatbots. It allows seamless integration of custom Node-based functions and tools into the conversation model, providing developers with a powerful and flexible way to enrich chatbot interactions.

With **AIChatEnhancer**, developers can incorporate external functions that can be dynamically invoked during conversations, enabling further customization of the user experience. From integrating complex logic to triggering custom tools, this tool offers unprecedented control over chatbot interactions within Godot.


<p align="center">
  
<img src="AI-Chat-Enhacer.png" alt="AI-Chat-Enhacer" width="400"/>

</p>


**AIChatEnhancer** makes it easy to extend your chat model with real-time function calling, enabling your chatbot to perform actions and access custom functionality during conversations. It allows developers to integrate external systems and logic into the flow of the chat, making it a powerful addition for more dynamic and responsive AI systems.

This tool connects directly to chat models like Ollama (or other similar models) via HTTP requests, without requiring additional assets (like GoPilot Utils). However, if you wish to use advanced UI features for managing the model or tools within the Godot editor, you can also install **GoPilot Utils** asset, though it is not required for basic functionality.

## Features
- Integrates custom functions into chatbot interactions within Godot Engine.
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
