This is just API connect from frontend and retrieve two inputs
To make sure you can run this in local server, you need to follow these steps:

1. open localhost://3000 main local server
2. in seperate terminal
3. Set Up a Python Virtual Environment
  In your root project (outside of /src), run:
 
  python -m venv venv
  
  source venv/bin/activate  # or `venv\Scripts\activate` on Windows
4.	Install FastAPI & Uvicorn

    pip install fastapi uvicorn

5.
   uvicorn python_fastapi.fetch_req_diagramType:app --reload
  
// here need to be careful if your python folder is python_fastAPI_fetch_clean and you can get fetch_req_diagramType function run 

7. type this in terminal fo testing //make sure you are in python_fastAPI_fetch_clean dir run this

curl -X POST http://localhost:8000/api/fetch_req_diagramType -H "Content-Type: application/json" -d "{\"requirement\":\"Build a login flow for admin dashboard. The user enters credentials, submits them, the system verifies, and redirects to the dashboard upon success.\", \"diagram_type\":\"sequence\"}"


-------this below just another way to run the test---------

7.or copy paste below test code for testing in the localhost://8000/docs

{
  "requirement": "Build a login flow for admin dashboard. The user enters credentials, submits them, the system verifies, and redirects to the dashboard upon success.",
  "diagram_type": "sequence"
}


