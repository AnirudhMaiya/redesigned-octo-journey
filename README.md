# idea for codefundo++
1. We are planning to come up with a mathematical modal which predicts areas that are prone to "Flooding" based on their rating.Higher the rating, higher are the chances of disaster.
2. The prediction is calculated based on causes such as:
	1. **Rainfall** in the area
	2. The **Elevation** of the area
	3. Intensity of **Clouds** in the area at a given time which can cause **Cloudbursts**
	4. Number of **Trees** in that area which helps in preventing floods
  	5. Whether the area is along the **Coastal** region
	6. Whether the area is near a **River** source
	7. Functioning **Sewage** pipelines in the area
	8. Whether the area is close to seas and has an epicentre for **Earthquake** which in turn creates **Tsunamis**
	9. Whether the area is **previously affected** by floods
	10. Whether the area is close to any **Mountain**, which can cause flooding when the glacier 
	on the mountain melts	
3. The outline of the mathematical model is as follows:<br>
  * Suppose there are **N** causes which creates a water-borne disaster like flood.
  * For each of these **N** causes, let **p<sub>1</sub>** ,**p<sub>2</sub>**, **p<sub>3</sub>** ,**p<sub>4</sub>**,.... **p<sub>N</sub>**  be the 	    **chance** or **probability** of that cause causing a disaster. 
  * Let **I<sub>1</sub>**, **I<sub>2</sub>**, **I<sub>3</sub>**, **I<sub>4</sub>** .... **I<sub>N</sub>** be the **Intensity** of each of the causes since every cause has a different level of damage in different areas (e.g.  For areas along the river source, the probability of river causing floods is more and for other areas which are not near a river source it is negligible) 
* Let **f** be the rating disaster in each area. (**higher the f value higher is the chance of flood disaster**)
* Basically **p** denotes chances and **I** denotes HOW MUCH ARE THE CHANCES feasible in that area

General Mathematical Model

Cause 1:&emsp;     **p<sub>1</sub>**&emsp;&emsp;(chance or probability of this cause creating a water-borne disaster)

Cause 2:&emsp;     **p<sub>2</sub>**&emsp;&emsp;(chance or probability of this cause creating a water-borne disaster)
      .<br>
      .<br>
      .<br>
      .<br>
Cause N:&emsp;    **p<sub>N</sub>**

-----------------   
&emsp; &emsp; ![first equation](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20P_i%20%3D%201)
-----------------


Now let us isolate an area

Cause 1:&emsp;   **I<sub>1</sub>**  &emsp;&emsp;                      (intensity of cause 1 in that area)&emsp;      I<sub>1</sub> ∈ [0,1]

Cause 2:&emsp;   **I<sub>2</sub>**  &emsp;&emsp;                      (intensity of cause 2 in that area)&emsp;      I<sub>2</sub> ∈ [0,1]
                  .<br>
                  .<br>
		  .<br>
 Cause N:&emsp;  **I<sub>N</sub>** &emsp;&emsp;                      (intensity of cause N in that area) 

--------------------

 If we take the product of **intensity** and **probability** of causes in one particular area we get the disaster rating
 
![second element](https://latex.codecogs.com/gif.latex?f%20%3D%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20I_i%20%5Ctimes%20P_i)<br>
*where f is the disaster rating of one particular area. Higher the f value, higher are the chances of flood disaster.*

4. Users can contribute by mapping all the trees in an area which are useful in preventing floods. This in turn has two advantages:
&emsp;* By calculating the number of trees in an area, 

5. The datasets used are:	
1. Layout of the functioning sewage pipelines from the local administrative body.	
2. Data of previous floods in an area from National Disaster Management Authority	
3. Data of earthquake prone areas from National Disaster Management Authority
6. The technology used are:
&emsp; 1. Satellite imagery from Google Maps to find elevation of an area, river, ocean sources and mountains close to an area.
&emsp; 2. Images of intensity of clouds and rainfall using satellite imagery from Accuweather.
	




