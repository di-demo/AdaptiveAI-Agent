Adaptive Knowledge based AI powered agent to aid human cognition and act as a highly integrated personal assistant by creating data orchestration layer that handles the following areas:  
### apply qualitative data filters on huge data volumes
separate data from noise 
transform data -> information -> knowledge
extract meta-knowledge from knowledge

# Current Architecture
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)


# Sample Use Case
fruit-detection
To predict the fruits and vegetables and the probability of freshness by loading a Keras model into memory using the Flask web framework to create an endpoint for our API to make predictions using our model, JSON-ify them, and return the results to the client, Option exists to call our Keras REST API using both cURL and Python

Usage
Start the server: python dnnServer.py Submit a request via cURL: curl -X POST -F image=@apple-3.jpg 'http://localhost:5000/predict' Submit a request via Python: python imgRecognition.py

Sample Results:
curl -X POST -F image=@orange-1.jpg 'http://localhost:5000/predict' {"predictions":[{"label":"orange","probability":0.9966147541999817}],"success":true}

curl -X POST -F image=@pom-1.jpg 'http://localhost:5000/predict' {"predictions":[{"label":"pomegranate","probability":0.9906478524208069}],"success":true}

curl -X POST -F image=@orange-apple-banana.jpg 'http://localhost:5000/predict' {"predictions":[{"label":"banana","probability":0.395834356546402},{"label":"lemon","probability":0.2627790570259094},{"label":"orange","probability":0.15947553515434265},{"label":"spaghetti_squash","probability":0.048288024961948395},{"label":"strawberry","probability":0.02415132336318493}],"success":true}

curl -X POST -F image=@apple-red.jpg 'http://localhost:5000/predict' {"predictions":[{"label":"Granny_Smith","probability":0.3485465943813324}],"success":true}

curl -X POST -F image=@capsicum.jpg 'http://localhost:5000/predict' {"predictions":[{"label":"bell_pepper","probability":0.9999898672103882}],"success":true}
