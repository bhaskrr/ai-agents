# AI Agents

## Intelligent Customer Service Agent

In today's fast-paced business environment, efficient and accurate customer support is crucial. Automating the initial stages of customer interaction can significantly reduce response times and improve overall customer satisfaction. This project aims to showcase how advanced language models and graph-based workflows can be combined to create a sophisticated support system that can handle a variety of customer inquiries.

### Key Components

1. State Management: Using TypedDict to define and manage the state of each customer interaction.

2. Query Categorization: Classifying customer queries into Technical, Billing, or General categories.
3. Sentiment Analysis: Determining the emotional tone of customer queries.
4. Response Generation: Creating appropriate responses based on the query category.
5. Escalation Mechanism: Automatically escalating queries with negative sentiment to human agents.
6. Workflow Graph: Utilizing LangGraph to create a flexible and extensible workflow.

### Method Details

1. Initialization: Set up the environment and import necessary libraries.

2. State Definition: Create a structure to hold query information, category, sentiment, and response.
3. Node Functions: Implement functions for categorization, sentiment analysis, and response generation.
4. Graph Construction: Use StateGraph to define the workflow, adding nodes and edges to represent the support process.
5. Conditional Routing: Implement logic to route queries based on their category and sentiment.
6. Database Integration: Saves the user interactions, query metadata, and response logs for analysis and continuous improvement.
7. Workflow Compilation: Compile the graph into an executable application.
8. Execution: Process customer queries through the workflow and retrieve results.

### Requirements

- python 3.10+
- python-dotenv
- langchain
- langchain_groq
- langGraph
- pymongo

### Graph Structure

![Graph Structure](./customer_service_agent_graph.png)

### Sample Mongo Database Documents

![alt text](./customer_service_data_mongo.png)

### Conclusion

By combining natural language processing capabilities with a structured graph-based approach, we've created a customer support agent that can efficiently handle a wide range of queries. This system can be further extended and customized to meet specific business needs, potentially integrating with existing customer support tools and databases for even more sophisticated interactions.
