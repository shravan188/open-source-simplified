# Open Source Simplified - Roadmap 1 

This roadmap is based on an open source project which is used by thousands of people. The open source project name will be revealed only to those who complete all the exercises and the capstone project

## Roles/Skillsets
If you are looking for internships/jobs, these are roles you can apply to if you complete this roadmap
* Python backend developer (FastAPI)
* Gen AI developer

## What is special about this roadmap?
* **This is NOT a generic roadmap**. This roadmap is exclusively based on one open source project, which is used by thousands of people, and only covers topics and subtopics relevant to that project. Completing this roadmap will enable you to reach a skill level where you can easily contribute to that project(and as a side effect other projects which use similar technologies)
* No spoonfeeding - while you will be given topics and exercises, there will be no tutorials. You will have to use the learning resources shared, or any other resource of your choice and solve the exercises.
* Cash prizes - First person to complete all exercises + capstone project + hidden task will win Rs 400, second person Rs 300 and third person Rs 200 (code sharing strictly not tolerated and will lead to immediate disqualification). People who complete after that will still get non monetary benefits like guidance to contribute to open source repositories
  
## Points to Note (Do not skip this)
1. Do not get stuck in tutorial hell Just learn what you need on the go. My prefered approach is
   * Step 1 : Start any topic with a quickstart docs (prefered) or a short quickstart video (less than 25 mins)
   * Step 2 : Directly jump into the exercise. Look at the reference code and if there is any line in the reference code you do not understand then just read the docs for that concept. Make notes as you learn
   * Step 3 : Use your learnings to solve the exercise
   * Step 4 : Submit your exercise and move to the next topic

2. Always read the official docs first. Go for video tutorial only if you do not understand docs. Many libraries have really good official docs. For example, FastAPI docs are really good. This is important because in the real world, you will have to use niche tools and libraries which will not have any video tutorials and will only have docs

3. Make notes as you learn. These will come in very handy afterwards
   
4. Have a goal - something which will push you when the going is not smooth. It could be getting an internship/job, being an open source contributor, just wanting to master something new etc. One major perk of completing this roadmap is you get to be part of an awesome AI community that is building cutting edge solutions for various India specific problems. So you can make a huge impact on the society as well, if you complete this, apart from all the other benefits.

5. If you have a doubt, google it. That should solve it 99% of the times. If that still does not help, ask your doubt in the discussions section, and someone might answer it   
  



# Roadmap Topics
## Python Fundamentals
### Concepts
1. Variables
2. Data Types (including int, str, list, dictionary, tuple, set)
3. Control Flow (if-else, for, while)
4. Functions
5. Object Oriented Programming basics
6. Generators

### Learning Material
1. https://github.com/Asabeneh/30-Days-Of-Python
   
### Exercise
Solve exercises from learning material 1 until you feel confident with your Python skills

## Package management
### Concepts
1. pip
2. Creating virtual environment
3. poetry
   
### Learning Material
1. https://python-poetry.org/docs/#installing-with-the-official-installer (for Poetry installation)
2. https://www.youtube.com/watch?v=5lioBm8f324 (for Poetry Windows installation)
3. https://github.com/Asabeneh/30-Days-Of-Python/blob/master/23_Day_Virtual_environment/23_virtual_environment.md
4. https://python-poetry.org/docs/basic-usage/

### Exercise
**Level 1** <br/>
Create a new project folder called virtual-environment-demo using poetry new. Inside the folder create a virtual environment using virtualenv library. Activate that virtual environment. Then use poetry to install the FastAPI package. Use the appropriate poetry command, list all installed packages within the virtual environment
<br/>
**Level 2**<br/>
Deactivate and delete the virtual environment. Create a new virtual environment and activate it. Install packages using the pyproject.toml file. Using poetry, list all installed packages within the virtual environment

<br/>

**Submission Guidelines**: Submission should be a Github link having the following
1. A text file listing all the commands used to solve the exercise
2. A screenshot of the terminal which lists all the installed packages
<br/>

<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>


## Web Concepts: Client, Server and API
This section is only to understand the thoery. Seeing learning material 1 should be sufficient for this section
### Concepts
1. What is a client
2. What is a server
3. Client server model vs peer to peer model

### Learning Material
1. https://www.youtube.com/watch?v=L5BlpPU_muY

### Exercise
None for this section

## FastAPI 
### Concepts
1. Creating a basic app which responds to GET request
2. Types, type hints and Pydantic models
3. Path and path operations
4. Response model
5. Routers (including prefix)
6. Dependency injection
7. Lifespan events
  
### Learning Material
1. https://fastapi.tiangolo.com/#create-it (start with this)
2. https://fastapi.tiangolo.com/learn/ (Fast API docs) 
3. https://www.youtube.com/watch?v=D-3JJLpECGQ (for routers)

### Exercise
Build a simple FastAPI app which satisfies the following conditions
1. The base url should return {"Hello":"World"}
2. When the user visits the route /v1/languages , it should return `{"languages":["en", "hi"]}`. This route should be in a separate file called languages.py and not in the main file i.e. main.py (Hint: Use routers)
3. The overall folder structure should be as follows
```
├── core
│   ├── __init__.py
│   ├── api
|   |   ├── languages.py
|   |   ├── __init__.py
├── main.py
├── venv
├── pyproject.toml
└── .gitignore
```
Make sure to use a virtual environment and Poetry to install packages <br/>
Reference code : https://medium.com/@mlopsengineer/routers-in-fastapi-tutorial-2-adf3e505fdca <br/>
**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code
2. Screenshot of response in the Swagger UI (localhost:8000/docs)
<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>


## Databases and ORM (SQLite and SQLAlchemy)
### Concepts
1. Database fundamentals - Relational vs NoSQL databases
2. What is SQLite and Installation 
3. Sorting and Filtering data using SQL
4. CRUD Operations using SQL (including create, insert, update, delete, replace)
5. ORM (understanding difference b/w orm and raw sql)
6. SQLAlchemy Engine and Session
7. Transactions and Operations (including read, write, commit, rollback)
8. Metadata, Table and Column (including what is metadata, column datatypes like Integer, String)
9. Working with data using SQLAlchemy ORM (including insert, select, update, delete)
    
### Learning Material
1. https://www.sqlitetutorial.net/
2. https://www.sqlitetutorial.net/what-is-sqlite/
3. https://docs.sqlalchemy.org/en/20/tutorial/
   
### Exercise
**Level 1** <br/>
Build a FastAPI app which connects to a SQLite database named db, with the following requirement 
1. Create a model called Transcription, which has the following fields : id (integer), user_id(integer), transcription(string), processed_text(string), word_count(integer), language(string). The word_count field must have a default value of zero, and the language column must have a value.
2. Create an endpoint `/v1/transcriptions`, which returns all the transcriptions.
3. Create another endpoint `/v1/transcriptions/save`, where user can pass user_id and language, and that entry gets added to the SQLite database. Try to use dependency injection to start the SQLalchemy session <br/>

**Reference code** : Code in the first 3 minutes of https://www.youtube.com/watch?v=cH0immwfykI <br/>

**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code
2. Screenshot of response in the Swagger UI (localhost:8000/docs)
<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>

## Asynchronous Python (including Asynchronous SQLAlchemy)
Note: This is a hard topic, so if you are not able to grasp this fully, just go ahead, and you can come back to it at a later point of time
### Concepts
1. Event Loop
2. Coroutines, Asyncio, Async and Await
3. Making SQLAlchemy code asynchronous (Refer https://www.youtube.com/watch?v=cH0immwfykI)

### Exercise
Convert the FastAPI app created in the Databases and ORM section from synchronous to asynchronous <br/>
Reference code: https://github.com/PrettyPrinted/youtube_video_code/blob/master/2023/05/27/How%20to%20Use%20Async%20SQLAlchemy%20in%20FastAPI/fastapi_async_sqlalchemy/app.py <br/>

**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code
2. Screenshot of response in the Swagger UI (localhost:8000/docs)

<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>

## Websockets
### Concepts
1. Websockets vs HTTP (including lifecycle of websocket, websocket url, pros and cons of web socket)
2. Building simple websocket client server using Python websockets library
3. Using websockets in FastAPI (refer https://fastapi.tiangolo.com/advanced/websockets/)

### Learning Material
1. https://apmonitor.com/dde/index.php/Main/WebSocketTransfer
2. https://fastapi.tiangolo.com/advanced/websockets/

### Exercise
**Level 1** </br>
Complete the activity shown in https://apmonitor.com/dde/index.php/Main/WebSocketTransfer
**Level 2** </br>
Build a simple messaging app between multiple clients using FastAPI and websockets. You can refer to the code in FastAPI docs, but do make sure to add one additional feature of your own

**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code

<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>

## Redis
### Concepts
1. Key value store 
2. Installing Redis (if Windows, check out https://www.youtube.com/watch?v=DLKzd3bvgt8)
3. Redis data types (including string, hash, set, list)
4. Redis string commands (including get, set, mget, keys, exists, persist, expire)
5. Redis hash commands (including hset, hget, hmget, etc)
6. Using Redis with FastApi
   
### Learning Material
1. https://redis.io/learn/howtos/quick-start/cheat-sheet
2. https://www.youtube.com/watch?v=6nY-kci1rlo (Redis with FastAPI in 16mins)
3. https://stackoverflow.com/questions/3046001/what-does-document-oriented-vs-key-value-mean-when-talking-about-mongodb-vs-c
   
### Exercise
#### Level 1
In the terminal/command prompt, create 2 entries with hash datatype. Then retrieve all of them
#### Level 2
Create a FastAPI app which gets data from any of the public APIs in the link - https://github.com/public-apis/public-apis and then caches it using redis, so that when the end users call the same url, they get the same data instantaneously

**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code

<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>

## LLM and Prompt engineering
### Concepts
1. LLM basics
2. Calling LLM apis like OpenAI(paid) and Groq(free)
3. Types of messages (system, user, assistant)
4. Types of models
5. Zero shot, Few shot prompting
   
### Learning Material
1. https://platform.openai.com/docs/guides/text-generation
2. https://console.groq.com/docs/quickstart

### Exercise
#### Level 1
Write a simple code which calls LLama-3-8b-8192 model with a user message (any message of your choice) using the Groq API. The Groq API key must be stored in a separate .env file and loaded using the dotenv library
#### Level 2
Convert the above code into a class called MyGroq. The class should have 2 methods
1. Constructor method with one instance attribute called client, which is the Groq object
2. Method called inference, which takes the model_id and prompt as input and returns the response of the LLM API call as the output
Note: Why did I not name the class Groq, and if I want to do that, what can I do?

**Submission Guidelines** : Submission should be a Github link having the following
1. Entire code

<br/>
<a href="https://docs.google.com/forms/d/e/1FAIpQLSdTaO8BpC8hZ7hYHrPTo7S1o-lgyzaMNy3UIh8IWpG78zfRmQ/viewform"><img src="https://github.com/shravankshenoy/oss_learning_paths/blob/main/submit_button.png" width="120" /></a>

## Web Authentication
1. Authentication vs Authorization
2. Session vs Token based authentication
3. JWT (including header, payload, signature)
4. CORS Middleware

### Learning Material
1. https://www.youtube.com/watch?v=YpvcqxYiyNE

### Exercise
COMING SOON

## Uvicorn
COMING SOON

## Audio processing and Speech to Text Conversion
COMING SOON

# Capstone Project 
This capstone project is based on a real world open source project, which you can contribute to once you finish the capstone project
#### Level 1
Given the client code [index.html](https://pages.github.com/), create a FastAPI app with the following
1. An endpoint /v1/languages which when called return {"languages":["en","hi"]}
2. A websocket endpoint /v1/ws/transcription which receives text from the client, and extracts the user_id and language from the received text. It returns the following response back to the client via the websocket
   {
                   "message_id": str(uuid.uuid4()),
                   "text": <the first 20 characters of the audio>
                   "type": <language given by user>
   }

#### Level 2
To the app written in Level 1, add the following features
1. Create a model called Transcription with the following fields : id (integer), user_id(integer), transcription(string), processed_text(string), word_count(integer), language(string)
2. In the /v1/ws/transcription endpoint, add code to store the following set into a Redis database with the key as transcription:{user_id}
   {
                    "transcription": <audio file>              
   }
3. Create an endpoint /v1/transcription/save, which given a user_id, returns all the transcription data corresponding to that user from the Redis database
4. In the above endpoint, write code to add the user, along with their language and transcription data as a new row into a SQLite database by using the Transcription model created in step 1

# Final Task [Locked]
This task will be visible only to those who complete all the exercises and the Capstone project successfully. Completion of this task will result in winning prize money and other benefits (such as being a contributor in large open source projects)
