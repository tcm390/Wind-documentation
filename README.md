# Wind-documentation

| WindType  |  |
| ------------- | ------------- |
|&nbsp;&nbsp;&nbsp;&nbsp;spherical  | Wind zone only has an effect inside the radius, and has a falloff from the center towards the edge.  |
|central  | Wind zone only has an effect inside the radius, the wind direction is always from center to player, and also has a falloff from the center towards the edge.  |
|directional  | Wind zone affects the entire scene in one direction.  |


| direction  |  |
| ------------- | ------------- |
| direction of the Wind Zone (only active for Spherical and Directional)|
### direction: direction of the Wind Zone (only active for Spherical and Directional)
### radius: Radius of the Wind Zone (only active for Spherical and Central)
### position Center position of the Wind Zone (only active for Spherical and Central)
### windForce: The primary force applied to all objects affected by the Wind Zone
### noiseScale: The value represents the noise of the wind. A greater value creates higher variation in wind direction.
### windFrequency: Defines the length and frequency of the wind pulses.


## Example:


     {
      "type": "application/wind",
      "content": {
        "windType": "directional",
        "direction": [0.5, 0, 0.2],
        "windForce": 0.5,
        "noiseScale": 1,
        "windFrequency": 1
      }
     }
      
     {
      "type": "application/wind",      
      "content": {      
        "windType": "central",        
        "direction": [0, 0.3, 0],        
        "radius": 5,        
        "position": [0, 0, -10],       
        "windForce": 5,      
        "noiseScale": 10,      
        "windFrequency": 10  
      }
     }
      
