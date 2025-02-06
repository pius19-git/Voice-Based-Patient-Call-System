# Voice-Based Patient Call System

## Model Download
Download the model from the following link and place it in the `model` folder:

[Model Link](https://drive.google.com/file/d/1OmjPWT6CziVi8liODIoDK-Avs3V-FJnn/view?usp=drivesdk)

---

## Running the Application Using Docker

### Steps:

#### 1. Build the Docker Container
To build the Docker container, run the following command:
```bash
sudo docker-compose build --no-cache
```
If `sudo` is not required on your system, you can use:
```bash
docker-compose build --no-cache
```

#### 2. Start the Docker Container
To start the container, execute:
```bash
sudo docker-compose up -d
```
Without `sudo`, use:
```bash
docker-compose up -d
```

#### 3. View Logs
To view logs of the running container, use:
```bash
sudo docker-compose logs -f
```
Without `sudo`:
```bash
docker-compose logs -f
```

#### 4. Access the API
Once the container is running, the API will be available at:
```
http://0.0.0.0:8000
```
For API documentation, visit:
```
http://0.0.0.0:8000/docs
```

---

## Running the Application Using Python Virtual Environment

### Steps:

#### 1. Create a Virtual Environment
To create a virtual environment, execute:
```bash
python3 -m venv env
```

#### 2. Activate the Virtual Environment
Activate the environment using the appropriate command for your operating system:

- **Linux/MacOS**:
  ```bash
  source env/bin/activate
  ```
- **Windows (Command Prompt)**:
  ```bash
  env\Scripts\activate
  ```
- **Windows (PowerShell)**:
  ```bash
  .\env\Scripts\Activate.ps1
  ```

#### 3. Install Requirements
Once activated, install the necessary dependencies:
```bash
pip install -r requirements.txt
```

#### 4. Run the Application with Uvicorn
To start the application, use:
```bash
uvicorn app:app --reload 
```

#### 5. Access the API
The API will be accessible at:
```
http://0.0.0.0:8000
```
For API documentation, visit:
```
http://0.0.0.0:8000/docs
```

#### 6. Stop the Application
To stop the running application, press:
```bash
Ctrl + C
```

---

## Notes
- Ensure that Python 3.7 or above is installed on your system.
- The `requirements.txt` file should include all the necessary dependencies to run the application.
- Place the downloaded model in the specified `model` directory before running the application.

---
