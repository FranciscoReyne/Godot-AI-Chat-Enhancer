# AIChatEnhancer
AIChatEnhancer is a tool that enhances AI chat systems by enabling dynamic tool integration and function calls. It supports advanced chat models, customizable system prompts, and optimized performance. Perfect for developers looking to integrate AI with custom tools in Godot.


¡Con gusto! Aquí tienes un `README.md` actualizado para tu repositorio de **AIChatEnhancer**:

```markdown
# AIChatEnhancer

**AIChatEnhancer** is a powerful tool designed to enhance and extend the functionality of AI chat systems, specifically for integration with tools and custom node functionalities. Built on top of Godot's AI architecture, this project allows for seamless tool interaction and function calling with advanced support for dynamic chat models.

## Features

- **Tool Integration**: Enables AI models to interact dynamically with custom tools and functions.
- **Enhanced Chat Model Support**: Supports AI models with built-in function calling (e.g., Llama3.1, Mistral Nemo, Hermes3).
- **Customizable System Prompts**: Easily modify system prompts to optimize AI behavior for specific tasks or use cases.
- **Optimized Performance**: Incorporates performance enhancements for efficient operation, even in complex tasks.
- **Interactive Interface**: Provides an intuitive interface for managing tool calls and monitoring AI interactions.

## Installation

1. Clone or download the repository:
   ```
   git clone https://github.com/yourusername/AIChatEnhancer.git
   ```
2. Follow the setup instructions in your Godot project:
   - Place the files in the `addons` folder of your Godot project.
   - Enable the plugin from the **Editor Settings** in Godot.

## Usage

Once installed, you can use **AIChatEnhancer** to enhance your AI chat systems. To start, instantiate the `ToolChatRequester` in your scene and configure the available tools.

### Example:
```gdscript
var chat_requester = ToolChatRequester.new()
chat_requester.target_node = $YourNode
chat_requester.tools = [your_tool_1, your_tool_2]
```

### API:
- `set_tool_active(function_name:String, active:bool)` – Set a specific tool's availability.
- `generate(prompt:String)` – Generate AI responses based on the current conversation.
- `call_tools(_tools:PackedStringArray, instruction:String)` – Call specific tools with instructions.

## Contributing

Feel free to fork this repository and submit pull requests with enhancements, bug fixes, or new features. Make sure to follow the [Code of Conduct](CODE_OF_CONDUCT.md) and ensure your changes are well-tested.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgments

- Thanks to the Godot Engine for providing the framework for this tool.
- Special thanks to the AI models and communities that made this project possible.

---

**AIChatEnhancer** is a flexible and powerful tool for creating advanced AI systems within the Godot engine. It’s ideal for developers looking to integrate custom AI tools or extend the capabilities of their chatbots.

---

Feel free to modify the content as needed and remember to replace `yourusername` in the GitHub clone URL.
