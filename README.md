# Retail-Query-Assistant
Retail Query Assistant is an application that converts natural language queries into SQL statements, specifically designed for retail data management. This project leverages advanced natural language processing technologies to make database querying accessible to users without SQL knowledge.


![](https://github.com/praj2408/Retail-Query-Assistant-Langchain-SQL/blob/main/docs/mysql-chains.png)



## Features
- Convert natural language to SQL queries
- User-friendly interface for entering natural language queries
- Support for various SQL databases
- Real-time query generation
## Technologies Used
- **LangChain:** Used for natural language processing and understanding.
- **OpenAI:** Utilized for its powerful language model to interpret and generate SQL queries from natural language.
- **Streamlit:** Provides an intuitive web interface for users to interact with the application.
- **SQL Database:** The backend database where generated SQL queries are executed

## Installation
To run Retail Query Assistant locally, follow these steps:

1. Clone the repository:
```
git clone https://github.com/yourusername/Retail-Query-Assistant.git
cd Retail-Query-Assistant
```

2. Set up a virtual environment:
```
conda create -n venv python==3.10 -y
conda activate venv
```

3. Install the required dependencies:
```
pip install -r requirements.txt
```

4. Set up environment variables:
Create a ".env" file in the project root and add your OpenAI API key:
```
OPENAI_API_KEY=your_openai_api_key
LANGCHAIN_API_KEY=your_langchain_api_key
LANGCHAIN_TRACING_V2=True 
OPENAI_MODEL_NAME=gpt-3.5-turbo-0125
```

5 Run the application:
```
streamlit run app.py
```

## Usage
1. Open your web browser and navigate to http://localhost:8501
2. The web app will open in your browser where you can ask questions
3. Click "Submit" to generate a SQL query using the database schema.
4. The generated SQL query will be applied to the database and shows the information on the app.

## Sample Questions
- How many total t shirts are left in total in stock?
- How many t-shirts do we have left for Nike in XS size and white color?
- How much is the total price of the inventory for all S-size t-shirts?
- How much sales amount will be generated if we sell all small size adidas shirts today after discounts?

## Contributing
We welcome contributions from the community! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes.
4. Commit your changes (git commit -m 'Add new feature').
5. Push to the branch (git push origin feature-branch).
6. Create a new Pull Request.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
