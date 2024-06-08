## VDA5050 Visualizer
The purpose of this package is to view and visualize vda5050 messages more quickly without looking at the json data. After running the application, you need to press the start button.


https://github.com/bekirbostanci/vda5050_visualizer/assets/26343575/06f22e56-1547-451b-97b9-870a715d525e


- Displaying the real-time position of multiple robots
- Displaying the vda5050 actions that robots perform
- Displaying data from the master controller to the robot and from the robot to the master controller 
- Display of raw json data 

## Live Demo

Check out the live demo of this project [here](https://vda5050-visualizer.vercel.app/).


## Install
Before than run app, please go to folder and install npm packages 
``` 
npm install 
```

## Run 
```
npm run dev
```

## MQTT Broker Settings 
Note Modern web browsers (google  chrome, firefox, opera etc.) cannot access the mqtt protocol directly. Therefore, if you want to use this application, please first enable the use of web sockets in your mqtt broker settings 

`
 sudo nano /etc/mosquitto/mosquitto.conf 
`
```
per_listener_settings true
listener 1883
allow_anonymous true

listener 14520
protocol websockets
allow_anonymous true
```


