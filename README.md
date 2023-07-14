# Influencer_identification_system

The influencer identification system is a tool that helps businesses identify potential influencers on Twitter based on their reach, engagement, and other metrics. The system uses natural language processing techniques to extract relevant features from tweets and analyze the behavior and characteristics of Twitter users.

## Requirements
To use the influencer identification system, you need to have the following installed:
- Docker
- Docker Compose
- Mysql

## Installation
1. download the docker desktop from this link https://www.docker.com/products/docker-desktop/

2. create a docker account following their steps 

3. navigate to the desktop of your computer in cmd
cd Desktop

4. Clone the repository:
Clone the repository: git clone https://github.com/your-username/influencer-identification-system.git

5. Navigate to the project directory and open it in vs code 

6. Create a .env file in the root directory of the project and define the required environment variables. Refer to the .env.example file for the list of variables and their format. ps(you can edit the .env file to add your database details)

4. Build and start the Docker containers:
docker-compose up --build

This command will build the Docker images and start the containers defined in the docker-compose.yml file. It will automatically set up the necessary services, including Node js and Mysql.
6. Access the influencer identification system app on http://localhost:3000 to view the identified influencers and insights.



# Contributors
Siddhesh Singh( sidd23heshsingh@gmail.com )
Dev Pratap Singh ( devpratapsingh122@gmail.com )
Vishnu Taparia ( vishnutaparia120@gmail.com )
Jairaj Singh ( jairaj.singh23@gmail.com )

# License
This project is licensed under the MIT License - see the LICENSE.md file for details.
