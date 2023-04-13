# Variables-Conditions-Tags

# Expected result yaml
QA branch
![image](https://user-images.githubusercontent.com/108743499/231871665-83a1b473-e601-4325-bac5-1240be2ca94f.png)
Main branch
![image](https://user-images.githubusercontent.com/108743499/231871778-1515f26f-b784-496f-ae2b-bb52496f768c.png)
Production branch
![image](https://user-images.githubusercontent.com/108743499/231872354-f8a272e7-6689-4ce6-93e4-35eef554ddc7.png)


# Release


If you need to use Artifact filters in your pipeline to make the deploy easier to te slot please follow the next steps

1- Go to https://dev.azure.com/{Your_Organization}/{Your_Project}/_release

2- Select your release pipeline and click in edit in the top right corner 
  ![image](https://user-images.githubusercontent.com/108743499/231868263-11e440e0-23c1-42f8-a6a6-a8ff9cb92f85.png)
  
3- Click in the Pre- deployment condition 
  ![image](https://user-images.githubusercontent.com/108743499/231868442-4b62fdc8-4b79-44d6-9bd7-a53343184083.png)
  
4- Go to Artifact filters and turn it on and then click in add 
  ![image](https://user-images.githubusercontent.com/108743499/231868595-aad5f80b-186d-4ec7-9825-113e869c5948.png)

5- Include the branches and the tags created in the example yaml
  ![image](https://user-images.githubusercontent.com/108743499/231868709-6a5ead9e-e649-4ae8-b1ec-e858f6e0581b.png)
  
 6- Make the some process in the others Stages and then based in the artifact filter select the slot to deploy the artifact 
 
  6.1 Go to the stage and click in the view stage task
      ![image](https://user-images.githubusercontent.com/108743499/231869016-50b19cbe-b2a6-4def-81e7-8bc37f59026e.png)
  
  6.2 Go to your deploy task and select your slot 
      ![image](https://user-images.githubusercontent.com/108743499/231869203-0e78dbc3-a4ac-4b05-85d9-1c6be2a7e518.png)
      
7- Save the release in the top right corner 
  ![image](https://user-images.githubusercontent.com/108743499/231869305-6de7fd05-096f-4455-a7dd-d81b1bfaf748.png)

 

