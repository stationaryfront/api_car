# api_car
MakeNTU workshop project

## Overview
We want to create a car that can
- be controlled by speech command
- recognize the sign on the road and make decision
using AI cloud cognitives APIs.

## Hardware Components
- toy car
- Raspberry Pi
- Picamera
- microphone(laptop)
- RFID cards and sensor
- map(street model)

## Map(Street Model)
The map defines the scenario a car may encounter on the road. Basic component is a T-shaped crossroad with
- road sign saying "right" or "left" on the wall
- an RFID card placed on the floor

## Operation
There are 2 modes: speech mode and text recognition mode. In both mode, the car would stop at each crossroad, triggered by sensing the RFID card.

### speech mode
the car decides to turn right or left base on the speech instruction sent from user, which is trancripted using speech API.

### text recognition mode
the car uses camera to read the sign with text recognition API and turn.

 Basically the car switches between 2 states, "forward state" and "listen and turn state". In the beginning it's in "forward state". When the RFID card is sensed, it turns to "listen and turn state" and turns back to "forward state" after the turn finished.

## Speech API

## Text Recognition API

## Streaming
