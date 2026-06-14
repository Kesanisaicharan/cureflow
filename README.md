# cureflow# CureFlow

### Know your turn before your turn comes.

## Overview

CureFlow is a real-time clinic queue management system built to eliminate paper token slips and reduce patient uncertainty.

Receptionists can manage patient queues efficiently, while patients can view live queue status and estimated waiting times without repeatedly asking for updates.

## Features

### Receptionist Dashboard

* Add Patient
* Auto Generate Token
* View Queue
* Set Average Consultation Time
* Call Next Token

### Patient Waiting Room

* Current Token Being Served
* Patient Token Number
* Tokens Ahead
* Estimated Wait Time
* Live Queue Updates

### Real-Time Synchronization

All connected devices are updated instantly using Socket.io whenever the receptionist performs any queue action.

## Tech Stack

### Frontend

* React.js
* Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB

### Real-Time Communication

* Socket.io

## System Flow

1. Receptionist adds a patient.
2. System generates a unique token.
3. Patient enters waiting queue.
4. Receptionist clicks "Call Next".
5. Backend updates queue.
6. Socket.io broadcasts updated queue.
7. All patient screens update instantly.

## Wait Time Formula

Estimated Wait Time = Tokens Ahead × Average Consultation Time

Example:

Tokens Ahead = 4

Average Consultation Time = 10 Minutes

Estimated Wait Time = 40 Minutes

## Edge Cases Handled

* Empty Queue
* Duplicate Token Prevention
* Multiple Receptionists
* Simultaneous Patient Addition
* Double Click Protection
* Consultation Time Updates
* Patient Cancellation

## Future Enhancements

* WhatsApp Alerts
* SMS Notifications
* Doctor Dashboard
* Appointment Scheduling
* Queue Analytics

## Impact

* Reduced Waiting Anxiety
* Better Queue Transparency
* Faster Reception Operations
* Improved Patient Experience

## Team

Built for Queue Cure '26 Hackathon.
