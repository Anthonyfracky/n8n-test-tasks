# Option 1: Low (Basic Level)

1. No-code/low-code platforms are tools that let people build software without writing much traditional code. They've become popular because they save time and money while allowing non-technical people to build applications. Like n8n

2. API is an Application Programming Interface functions. It takes requests from one software, delivers them to another software, and returns the response back according to specific rules and formats. When you check weather on your phone, an API is working behind the scenes to get that data from a weather service. In our case, I worked with various APIs to get data, such as ClickUP or OpenAI.

3. JSON is a human-readable and machine-friendly way to format data. It uses a simple structure of key-value pairs that works universally across different platforms. A simple example would look like `{"name": "John", "age": 25}`. Its simplicity and versatility make it the go-to format for most modern APIs.

4. A webhook works like a notification system for applications. Instead of constantly checking for updates, the system automatically notifies you when something happens. This is particularly useful for real-time updates, like getting a Slack notification for example. I used it in my first practical task

5. OAuth2 is a security protocol that acts like a digital valet key. It allows users to give applications limited access to their data without sharing their actual credentials. This is the system you're using when you click "Sign in with Google" or "Login with Facebook" on various websites. In our case, this was the basis of my Google account verification in n8n.

# Option 2: Mid (Intermediate Level)

1. Error handling in workflow automation is about preparing for things to go wrong. It involves detecting errors, having backup plans, keeping logs for review, and making sure the right people know when problems occur. For instance, if an email fails to send, the system might try again after a few minutes.

2. REST API represents a set of rules for building web services. It uses standard HTTP methods like GET, POST, PUT, and DELETE, and can be tested using tools like Postman (I used it to send data in the first task). When you interact with a REST API, it returns status codes that tell you what happened with your request – 200 for success, 404 if something wasn't found, and so on.

3. ClickUp integration can transform task management by automating the creation of tasks from emails, keeping deadlines synced across teams, tracking time automatically, and generating reports without manual intervention.

4. When handling failed tasks in automation, you need a smart retry strategy. This might include trying again immediately, waiting longer between each attempt, setting a maximum number of retries. This ensures your automation is resilient and reliable.

5. Webhooks play a vital role in real-time processing because they eliminate the need for constant checking. Instead of repeatedly asking "Is there anything new?", webhooks tell you immediately when something happens. This makes systems more efficient and responsive.

# Option 3: Hard (Advanced Level)

1.  ETL (Extract-Transform-Load) is fundamental to modern data automation. In practice, it means taking data from various sources, converting it into a useful format, and placing it where it needs to go. A common example would be taking raw sales data from multiple stores, standardizing the format, and loading it into a central database for analysis. For example, I worked with ETL during one task when I was processing a database with information about users. I performed the extraction and transformation of the necessary properties and their subsequent aggregation into an updated database. I did it with Docker.

2.  Vector databases serve as specialized storage systems that represent data as mathematical vectors. They excel at finding similar items and are essential for modern AI applications. When you're trying to find similar images or text, vector databases can do this much faster than traditional databases because they understand the actual meaning and context of the data. I worked with this when I was doing the RAG project. There I used the FAISS vector database to store information

3.  Integrating third-party APIs without pre-built connectors requires a deep understanding of API documentation. You'll need to write your own HTTP requests, manage authentication yourself, and create comprehensive error handling. It's like building a custom bridge between two systems when there isn't already a road connecting them.

4.  Retry logic is all about persistence and smart timing in automation. When implementing it, you need to decide how many times to retry, how long to wait between attempts, and what to do with different types of errors. Some errors might need immediate retries, while others might benefit from longer waits between attempts.

5.  GPT-4 processes emails by understanding their context, determining importance, and extracting key information. It can understand email threads, suggest responses, and even identify action items. Think of it as a very smart assistant who can read your emails and tell you what's important and what needs to be done. In this task, we just implemented a small version where we used OpenAI to analyze emails for the presence of tasks in them.

6.  Complex workflows are like intricate automation chains where each step must execute correctly for the entire process to function smoothly. A good example is task management automation, where data is extracted from a project management tool, filtered based on priority, scheduled in a calendar, and then summarized in an email. Different conditions can lead to multiple branching paths, making the workflow dynamic and adaptable. I worked on automating task extraction from ClickUp, event creation in Google Calendar, and email notifications, ensuring seamless integration between different services with minimal manual input.

7.  Custom nodes are like creating your own tools when existing automation options don’t fully meet your needs. They are useful when you need to integrate with a unique API, apply custom logic, or process data in a specific way that standard nodes don’t support. Once built, they can be reused across multiple workflows, making automation more efficient. In my case, while working with n8n, I used JavaScript code nodes to filter and transform data from ClickUp tasks and process AI-generated outputs, which is a similar approach to creating a custom node for tailored functionality.

8.  Automation can revolutionize customer communication by providing instant responses to common questions, scheduling follow-ups at the right time, and personalizing messages at scale. It's like having a really efficient assistant who never sleeps and always remembers to follow up with customers at the right time.

9.  Integrating Google Sheets, Gmail, and n8n creates a powerful automation ecosystem. You can automatically collect email data, track responses, generate reports, and manage information centrally. For example, customer inquiries from Gmail can automatically populate a Google Sheet, which then triggers specific workflows in n8n.

10. When developing AI systems, key ethical considerations include bias and fairness; transparency, making AI decisions understandable and explainable; privacy and data security, protecting user data from misuse; and accountability, ensuring responsibility for AI-driven decisions. Additionally, AI should be designed to avoid harm, prevent misinformation, and respect user autonomy.
