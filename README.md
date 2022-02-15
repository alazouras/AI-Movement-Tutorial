# AI-Movement-Tutorial
Write up of how to code an NPC to walk to different places in an area

# 1) Setting up the terrain
To set up the scene, you can import a custom map from the Unity Asset store, but for this I will create my own for simplicity. It is important for this tutorial to have a Plane as well as objects (in this case cubes) that will be deemed "unwalkable" later. I have also given the obstacles a custom material so that they stand out, but this is optional:

![image](https://user-images.githubusercontent.com/91538155/154043197-33dca8e7-0470-499d-86ff-3afcb7972388.png)

Next, I add the Character, in this case a simple capsule with a material, and label it as CharacterAI. Here, also make sure to tag the NPC as any custom tag that will be connected to it being a Character, in this case I tagged it as NPC:

![image](https://user-images.githubusercontent.com/91538155/154043948-071e6ddd-8217-4450-abd9-7cbe8e659303.png)
![image](https://user-images.githubusercontent.com/91538155/154043899-2e6f6d9b-a5c9-4413-960e-c08f95445b82.png)

# 2) Setting up the NavMesh
To set up the NavMesh, go into Window -> AI -> Navigation

![image](https://user-images.githubusercontent.com/91538155/154048088-23ee1531-57ae-4689-ad6e-d3c2c4b24dba.png)

To get the NavMesh to work, click on the Plane and set it to Static, then Walkable, then Bake:

Then, click on all the obstacles, and then it's the same process except label it at Unwalkable:
