# SWIM Natural Language Narrative Generator 2.0
Automated generation of text-based explanations of SWIM model outputs.

## Features
- Narration of peak and minium values.
- Narration of high impact trends.
- Narration of comparison against contextual benchmarks.
- Narration of trends through simple moving averages.

## Build and Run

## Option 1: Docker Compose File
1. Download the docker-composer.yml file to a path in your machine.
2. Install Docker and Docker composer on your target machine.
3. Setup your docker account at: https://www.docker.com/get-started
4. Configure the docker-composer file with your own app settings.
5. Run docker compose: docker-compose up
    5a. Use -d option on the composer command to run on the background.
6. Swagger docs available at http://localhost:6040/api-docs


### Option 2: Build Docker Container
1. Download this repository into a folder on your machine.
2. Install Docker and Docker composer on your target machine.
3. Setup your docker account at: https://www.docker.com/get-started
4. Using a command line or terminal navigate to the base path of the project.
5. Build the image: > docker build -t swim-nlng:latest.
6. Modify the file docker-compose.yml accordingly.
7. Run the container: > docker-compose up
8. Once running, the API documentation will be locally available at http://localhost:5030/swagger

### Option 3: Native
For a native installation make sure to have Java and Maven installed on your target machine.   

1. To download dependencies and buld the project run > mvn clean install
2. Customize the settings.yml file accordingly
3. To run the service execute: java -jar ".\target\swim-nlng-2.0.0.jar" server settings.yml
4. Once running, the API documentation will be locally available at http://localhost:5030/swagger

## Contributors
Angel Ortega   
Luis Garnica  
Raul Alejandro Vargas Acosta    

## Acknowledgements
This material is based upon work supported by the National Science Foundation (NSF) under Grant No. 1835897.   

Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.

## How to cite
If you create products such as publications using SWIM products, it would be great if you add the ??following acknowledgement:   

"This work used the Sustainable Water for Integrated Modeling (SWIM) 2.0, which was supported by the National Science Foundation under Grant No. 1835897."  

Please use the following citation for this product:   
Vargas-Acosta, R. A., Chavira, L. G., Villanueva-Rosales, N., & Pennington, D. 
Towards SWIM Narratives for Sustainable Water Management. 

## License
This software code is licensed under the [GNU GENERAL PUBLIC LICENSE v3.0](./LICENSE) and uses third party libraries that are distributed under their own terms (see [LICENSE-3RD-PARTY.md](./LICENSE-3RD-PARTY.md)).

## Copyright
?? 2015-2023 University of Texas at El Paso (SWIM Project) 
