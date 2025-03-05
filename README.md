# Chain of Thought Simulation - n8n Workflow

## Overview
This n8n workflow is designed to simulate advanced chain-of-thought reasoning using multiple prompting techniques and API calls. It leverages lightweight non-thinking LLMs like Google Gemini Flash 2.0 to mimic the behavior of more advanced reasoning LLMs such as DeepSeek R1 or OpenAI o3-mini-high.

The workflow constructs multi-step reasoning chains, progressively refining responses through structured processing, auto-parsing, and iterative feedback loops.

## Features
- **Simulated Chain of Thought (CoT):** Uses step-by-step logic refinement to mimic reasoning LLMs.
- **Multi-Prompt Processing:** Breaks down complex questions into sub-tasks and reassembles them into final conclusions.
- **Automated API Calls:** Interfaces with Google Gemini and Groq API to enhance processing speed and accuracy.
- **Error Handling & Refinement:** Uses auto-fixing nodes to correct inconsistencies and refine responses.
- **Structured Outputs:** Utilizes n8n output parsers to ensure clean and interpretable results.

## Setup Instructions

### Prerequisites
- n8n installed (via Docker, npm, or cloud instance).
- API credentials for Groq and Google Gemini (PaLM).

### Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/n8n-workflow.git
   ```
2. Navigate to the project directory:
   ```sh
   cd n8n-workflow
   ```
3. Import the workflow:
   - In n8n, navigate to **"Workflows" > "Import from File"**.
   - Select `workflow.json` and upload it.
4. Set Up API Credentials:
   - In n8n, go to **"Credentials"** and add your API keys for Groq and Google Gemini.
   - Ensure that the credential names match those referenced in the workflow.
5. Activate the Workflow:
   - Enable the workflow and start testing!

## File Structure
```
📁 n8n-workflow
├── README.md          # Documentation
├── LICENSE            # MIT License
├── .gitignore         # Ignore unnecessary files
└── workflow.json      # The exported n8n workflow (sanitized)
```

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Contributions
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions.

## Disclaimer
This workflow does not include API keys. Ensure you add your own credentials securely in n8n.
