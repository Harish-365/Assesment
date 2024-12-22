<<<<<<< HEAD
# CloudEngine Labs DevOps & Cloud Engineer Assignment

## Time limit

- Assignment needs to be submitted **within 2 days** after it is shared to candidate.

## Objective of the assignment 

- This is to test the basic understanding of candidate's knowledge in the below areas,

1. Git commands usage
2. Knowledge on Containers
3. Testing whether the candidate providing attention to necessary details as part of implementation

## Instructions

**Please read and follow the instructions carefully**

### Create Repo in your GitHub account

- Please create an user account in GitHub, if you don't have one.
- Create new repo in your GitHub to complete the assessment
- Alternatively you can clone this repo and add your code

### Assignment problem statements

#### Must have requirements (for Junior Roles)

- [ ] Step 1: Create a simple Python program to print, `"Hello cloud-engine labs!!"`
- [ ] Step 2: Create a `Dockerfile` in the project to create a container image for the program in the repo
- [ ] Step 3: Test the `Dockerfile` by building the image 
- [ ] Step 4: Run the image as a container. It should print the string `"Hello, cloud-engine labs!!"`
- [ ] Step 5: Commit and Push the updated code into your GitHub repo

#### Good to have requirements (Must for Senior Roles)

- [ ] Step 6: If you're able to create a `GitHub Action` workflow for the Docker CI automation, then you have an added advantage for the submission.
- [ ] Step 7: Push the image into any container registry and share the image name as part of deliverable.
- [ ] Step 8: Run the container image on a specific port (of your choice)
- [ ] Step 9: Create docker-compose file and use the image from container registry 

### How to submit

- Capture the output of **All the Steps** in a _Google Document_ (If you can create the steps in README.md files that is good)
- Clearly mention the steps you have completed in your final documentation
- Share repository link from your GitHub account
- Share the google document link or README file link to [work@cloudenginelabs.io](mailto:work@cloudenginelabs.io)

Note:

- Anytime if you have questions, please drop a note to [work@cloudenginelabs.io](mailto:work@cloudenginelabs.io)
=======
# Assesment

Step 1: Create a Simple Python Program
Created a file named hello.py with the following content:

python
print("Hello cloud-engine labs!!")

Step 2: Create a Dockerfile
Created a file named Dockerfile in the same directory as your hello.py file with the following content:

Dockerfile
Use an official Python runtime as a parent image
FROM python:3.8-slim

Set the working directory in the container
WORKDIR /app

Copy the current directory contents into the container at /app
COPY . /app

Run hello.py when the container launches
CMD ["python", "hello.py"]

Step 3: Test the Dockerfile by Building the Image
Run the following command to build the Docker image:
bash
docker build -t hello-cloud-engine-labs .

Step 4: Run the Image as a Container
Run the following command to start a container from the image:
bash
docker run hello-cloud-engine-labs

Step 5: Commit and Push the Updated Code into Your GitHub Repo
bash
git init

bash
git add .
Commit the Changes:

bash
git commit -m "Add hello.py and Dockerfile"


bash
git remote add origin https://github.com/Harish-365/Assesment
Push the Changes to GitHub:

bash
git push -u origin main


