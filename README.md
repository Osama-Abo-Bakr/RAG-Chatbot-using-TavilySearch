# RAG-Chatbot-using-TavilySearch

A Retrieval-Augmented Generation (RAG) chatbot built using TavilySearch and LangChain, designed to respond to user queries with precise, well-structured answers in Markdown format. The chatbot leverages the TavilySearch tool to retrieve relevant web-based information and presents it via a Streamlit application.

## Features

- **Integration with TavilySearch**: Uses TavilySearchResults for retrieving web-based data to enhance responses.
- **Markdown Formatting**: Outputs responses in clean Markdown format with headings, lists, tables, and code blocks for better readability.
- **Streamlit Interface**: Provides a user-friendly web interface for asking queries and viewing responses.
- **Tool-Assisted Responses**: Employs LangChain’s tool-calling agents for dynamic query resolution.

## Technologies Used

- **Python**
- **Streamlit**: For creating the web-based user interface.
- **LangChain**: Framework for building tool-augmented chatbots.
- **TavilySearchResults**: Tool for retrieving web search results.
- **ChatGroq**: AI model for generating conversational responses.
- **dotenv**: For managing environment variables.

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:

   ```bash
   git clone https://github.com/Osama-Abo-Bakr/RAG-Chatbot-using-TavilySearch.git
   cd RAG-Chatbot-using-TavilySearch
   ```

2. Set up a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file and set up your environment variables. For example:

   ```
   OPENAI_API_KEY=your_openai_api_key
   TAVILY_API_KEY=your_tavily_api_key
   ```

## Usage

1. Run the application:

   ```bash
   streamlit run app.py
   ```

2. Open your web browser and navigate to `http://localhost:8501`.

3. Enter your query in the chat input box and receive well-structured responses.

## Code Overview

### `response_to_json(user_query)`

This function:
- Integrates the TavilySearchResults tool for web searches.
- Uses LangChain to create a tool-calling agent with a custom prompt.
- Executes the agent to generate responses based on user input.

### `main()`

This function:
- Loads environment variables.
- Configures the Streamlit interface.
- Handles user queries and displays both user input and the chatbot’s responses.

## Example Query

1. Input: `What are the benefits of machine learning?`
2. Output:

   ```markdown
   # Benefits of Machine Learning

   - Automates repetitive tasks.
   - Enhances decision-making processes.
   - Improves efficiency in various industries.

   ```

## Contributing

Contributions are welcome! Please fork the repository and create a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or support, feel free to reach out:
- **GitHub**: [Osama-Abo-Bakr](https://github.com/Osama-Abo-Bakr)

---

Enjoy building and exploring with the RAG-Chatbot!