# idea for codefundo++
1. We are planning to come up with a mathematical modal which predicts areas that are prone to "Flooding" based on their rating.Higher the rating, higher are the chances of disaster.
2. The prediction is calculated based on causes such as:
	1. Rainfall in the area
	2. The Elevation of the area
	3. Intensity of “Clouds” in the area at a given time which can cause “Cloudbursts”
	4. Number of "Trees" in that area which helps in preventing flood
  	5. Whether the area is along the "Coastal" region
	6. Whether the area is near a "River" source
	7. Functioning "Sewage" pipelines in the area
	8. Whether the area is close to seas and has an epicentre for "Earthquake" which in turn creates Tsunamis
	9. Whether the area is previously affected by floods
	10. Whether the area is close to any "Mountain", which can cause flooding when the glacier 
	on the mountain melts	
3. The outline of the mathematical model is as follows:<br>
  * Suppose there are 'N' causes which creates a water-borne disaster like flood.
  * For each of these 'N' causes, let p<sub>1</sub> ,p<sub>2</sub>, p<sub>3</sub> ,p<sub>4</sub>,.... p<sub>N</sub>  be the 	    Chance or Probability of that Cause causing a Disaster. 
  * Let I<sub>1</sub>, I<sub>2</sub>, I<sub>3</sub>, I<sub>4</sub> .... I<sub>N</sub> be the Intensity of each of the causes since every cause has a different level of damage in different areas (e.g.  For areas along the river source, the probability of river causing floods is more and for other areas which are not near a river source it is negligible) 
* Let f be the rating disaster in each area. (higher the f value higher is the chance of flood disaster)
* Basically p denotes chances and I denotes HOW MUCH ARE THE CHANCES feasible in that area
<br>
<pre>
General Mathematical Model:
Cause 1:     p<sub>1</sub>               (chance or probability of this cause creating a water-borne disaster)
Cause 2:     p<sub>2</sub>               (chance or probability of this cause creating a water-borne disaster)
                  .
                  .
                  .
Cause N:     p<sub>N</sub> 
-----------------   
</pre>
![first example](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20P%20%3D%201)

Now let us isolate an area. 
Cause 1:   I1                        (intensity of cause 1 in that area)      I1 ∈ [0,1]
Cause 2:   I2                        (intensity of cause 2 in that area)       I2 ∈[0,1]
                  .
                  . 
 Cause N:  IN                       (intensity of cause N in that area) 
 
https://latex.codecogs.com/gif.latex?f%20%3D%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20I_i%20%5Ctimes%20P_i

where f is the disaster rating of each area. Higher the f value, higher are the chances of flood disaster.

Users can contribute by mapping all the trees in an area which are useful in preventing floods.  
The datasets used are:
	Layout of the functioning sewage pipelines from the local administrative body.
	Data of previous floods in an area from National Disaster Management Authority
	Data of earthquake prone areas from National Disaster Management Authority
The technology used are:
	Satellite imagery from Google Maps to find elevation of an area, river, ocean sources and mountains close to an area.
	Images of intensity of clouds and rainfall using satellite imagery from Accuweather.
	




