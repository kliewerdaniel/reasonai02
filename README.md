Reasoning AI 02

Welcome to Reasoning AI 02, an advanced AI agent framework designed to autonomously decompose complex tasks, reason through each step, and provide comprehensive outputs. This project leverages Next.js for the frontend interface and Ollama, an open-source local LLM runner, for executing AI models locally, ensuring privacy and eliminating API costs.

Features
	•	Step-Based Task Decomposition: Automatically breaks down user-defined goals into manageable steps for systematic execution.
	•	Reasoning Before Action: Provides transparent reasoning for each step before performing actions, enhancing clarity and trust.
	•	Streaming Progress Updates: Delivers real-time updates as the agent progresses through each step, keeping users informed.
	•	Contextual Memory: Maintains context throughout the task execution, ensuring coherence and relevance in outputs.

Prerequisites
	•	Node.js: Ensure you have Node.js installed.
	•	Ollama: Install Ollama to run local AI models.

Getting Started

1. Clone the Repository

git clone https://github.com/kliewerdaniel/reasonai02.git
cd reasonai02

2. Install Dependencies

npm install

3. Set Up Environment Variables

Create a .env file in the root directory to configure environment-specific variables.

4. Pull the Mistral Model with Ollama

Download the Mistral model to enable local AI processing:

ollama pull mistral

5. Run the Development Server

Start the Next.js development server:

npm run dev

Navigate to http://localhost:3000 in your browser to access the application.

Usage
	1.	Define a Goal: Enter a specific goal or task you want the AI agent to accomplish.
	2.	Observe Task Decomposition: The agent will break down the goal into clear, manageable steps.
	3.	Follow Reasoning and Execution: For each step, the agent will provide its reasoning and then execute the action, displaying the output.
	4.	Receive Final Output: After completing all steps, the agent will present a comprehensive result based on the initial goal.

Architecture Overview

The application consists of the following key components:
	•	Frontend: Built with Next.js, providing a responsive interface for user interaction.
	•	Agent Class: Implements the logic for task decomposition, reasoning, and step execution.
	•	Ollama Integration: Facilitates local execution of AI models, ensuring data privacy and reducing dependency on external APIs.

Customization

To tailor the agent’s behavior:
	•	Modify Task Decomposition Logic: Adjust how the agent breaks down tasks by editing the analyzeTask method in the Agent class.
	•	Enhance Reasoning Mechanism: Refine the agent’s reasoning process by updating the generateReasoning method.
	•	Integrate Additional Tools: Expand the agent’s capabilities by incorporating new tools or APIs into the execution steps.

Contributing

Contributions are welcome! To contribute:
	1.	Fork the repository.
	2.	Create a new branch (git checkout -b feature-branch).
	3.	Commit your changes (git commit -m 'Add new feature').
	4.	Push to the branch (git push origin feature-branch).
	5.	Open a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements

Special thanks to the developers of Ollama for providing the tools necessary to run local AI models efficiently.

⸻

For more detailed insights into building custom AI agent frameworks with Next.js and Ollama, refer to the blog post: Building a Custom AI Agent Framework with Next.js and Ollama.
