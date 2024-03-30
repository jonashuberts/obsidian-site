---
title: AI Car race
description: 
aliases: 
draft: true
tags: 
date: 27th March 2024
---
# Buttons
## Basic
- 🌎 Load World
- 📁 Load .car file
- 💾 Save .car file
## Car
- ⚙️ Change settings of the car
	- Ray Count: How many linear sensors should the car have
	- Ray Length: The length of the sensors
	- Ray Spread: The field of view of all angles
	- Ray Offset: The offset angle of the field of view
- 🛞 Manual drive 
- 🔄 Respawn car
## Training
- 🧬 Start a training round
- 💾 Save current red highlighted car mutation
- ❌ Close current training
- Slider: Controls the amount of change to the next mutation, a higher bar will increase the difference to the previous mutation and a lower bar will be more like the previous mutation.
## Nodes
- Button Ones:
	- The with the arrows are the sensor inputs
	- The Clock is the actual time
- Middle Ones:
	- Hidden Layers for combining different inputs to an output
- Upper Ones:
	- The Possible outputs of the model (drive forward, steer right, steer left, drive backwards)
- Editing Nodes:
	- Click a node but doesn't move it
	- Then you can drag a line to create a connection
	- You can either connect to an existing node or to a new hidden one by clicking in an empty space
	- Right-clicking deletes connections and nodes
- Weights:
	- By clicking a node or connection and using "+" and "-" you can change the weight of a specific node
# Training
## Idea
### Phase 1 (finish race)
1. Start a Training Round
2. Measure the distance travelled by the car
3. If it is a record save the current car
4. If it was the tent record since one was saved then save the current .car model
5. Start a New Training Round
6. Repeat a car has finished the whole race
### Phase 2 (time optimization)
1. Start a Training Round
2. Measure the time taken to complete the race
3. If it is a record, save the current car
4. If it was the tent record since one was saved then save the current .car model
5. Start a New Training Round