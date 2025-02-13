# PPJ 2 - Thomas Deolall
2/13/2025

## Tasks
- 2 hrs: Set up up GitHub repository and created the basic system for the heartbeat mechanic
- 15 min (in-class): Added functionality for early/late windows for the heartbeat system
- 1 hr: Full team meeting on 2/12/25. Discussed what everyone will work on in the coming weeks and tested working with multiple different branches on GitHub

## Blog
The main thing I did this week was create functionality for the heartbeat system. As mentioned in my contract, I want to ensure that system is modular and easily expandable, so I've made several parameters easily accessible and editable, even during runtime. These parameters include the starting size of the hit indication, how fast the hit indication shrinks, the BPM, and the size of the hit/miss windows. 

## Milestones
The final versions of the individual and team contracts were due. The team worked together to make revisions to the team contract. I referenced my aspects on the team contract to help build out the rest of my individual contract.

## Image(s)
![image](https://github.com/user-attachments/assets/8ef54530-346c-4d1c-bc38-921fb083198c)


## Looking Ahead
There are some minor issues with the current version of the heartbeat system, mainly stemming from the fact that I am simply shrinking an image to represent the hit indicator:
1. The variables responsible for denoting the hit/miss windows merely look at the current scale of the image, which isn't super intuitive when tweaking them. More importantly, this would also mean that the hit window is smaller when the hit indication shrinks fast compared to when it is slower.
2. The lines of the hit indication are much thicker when the image is larger, and much thinner when the image is smaller (Solution: Try using a vector image instead of raster??)

I would like to resolve these issues before moving away from the heartbeat system. Once done, I am going to implement the camera movement functionality when the player selects a hallucination event.
