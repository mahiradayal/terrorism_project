# Summary of Project

For this project, I used the Global Terrorism database which has infromation on attacks between 1970 and 2019 all around the world — which is 201,184 individual incidents. 

Each entry is labelled as one of the following categories: 
- Armed Assault 
- Assassination 
- Bombing/Explosion 
- Facility/Infrastructure Attack
- Hijacking 
- Hostage Taking (Barricade Incident)
- Hostage Taking (Kidnapping)
- Unarmed Assault
- Unknown

However, some of the Facility/Infrastructure attacks and hijackings are also bombings, so their categories need to be re-done. I was interested in classifying bombings and explosions in this dataset to predict whether or not an attack is a bombing. 

## Method 

I first created a column with boolean 0/1 values for whether the attack is classified as a bombing in the dataset. 

Then, to add in others which were left out, I added bombing/explosion related keywords to my training dataset — which included terms like “device,” “firebomb,” “explosive,” “detonate,” etc. 

I tried a Decision Tree Classifier, (0.7805392078892953), Nearest Centroid (0.7461825990138381)and BernoulliNB (0.780916971528551) to pick one with a high clf score.

The most important features were “explosive,” “bomb,” “detonate,” and “firebomb.”

## Next Steps

I plan to map all the exact locations of bombings, since I have the latitude and longitude for each of them. 

Some further analysis I could do: 
How likely is it for an attack to take place on a university campus, or within 1 mile of a university? 
How likely is it for a bomb blast or explosion to take place in a specific country? 
Each target area is also categorized, so I could look into common bomb blast targets. 
 
