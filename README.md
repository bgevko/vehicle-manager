# Vehicle Manager App User Flow

This is a text-based user flow for the vehicle manager, designed in accordance with how iOS navigation behaves. You get the feel for the user flow by looking at the available options on the screen, and clicking the link to navigate to a new screen.

- _Driver:_ The person using the vehicle
- _Manager_: The person managing assets and possibly using the vehicle
- _User_: Either driver or manager

Assuming Cancel / delete attempts will be met with appropriate prompts.

## Login

- User can log in and be redirected to the [Vehicles](#vehicles) screen
- User can register
- User can reset their password

## Vehicles

- User can go to [Trips](#trips)
- User can go to [Maintenance](#maintenance)
- User see the list of all vehicles, with available and checked out vehicles grouped separately.
  - Filterable by vehicle type, last driven, last driver, mileage, and maintenance status (Overdue, due soon, up-to-date)
- User can go to [Vehicle Details](#vehicle-details) by selecting a vehicle.
- User can single-tap checkout a vehicle; the state is updated appropriately
- User can see their checked out vehicle. User can go to [Begin Trip](#begin-trip) from their checked out vehicle.
- User can single-tap check in a vehicle; the state is updated appropriately
  - If a trip is in progress, the driver will be taken to the [End Trip](#end-trip) form
- Manager can assign/edit a vehicle to a driver using the [Assign Vehicle Form](#assign-vehicle-form)
- Manager can go to the [Manage Vehicles](#manage-vehicles) screen

## Assign Vehicle Form

- Manager can cancel, going back to the previous contextual screen.
- Manager can select a driver from a drop-down list of available drivers
- Manager can select a vehicle from a drop-down list of available vehicles
- Manager can confirm the assignment, going back to [Vehicles](#vehicles), or the previous contextual screen.

## Manage Vehicles

- Manager can go back to [Vehicles](#vehicles), or the previous contextual screen
- Manager can add a new vehicle with the [Vehicle Form](#vehicle-form)
- Manager can edit a vehicle with the [Vehicle Form](#vehicle-form)
- Manager can delete a vehicle.
- Manager can go to [Vehicle Details](#vehicle-details)

## Vehicle Form

- Manager can cancel, going back to [Vehicles](#vehicles) or the previous contextual page
- Manager can input the vehicle's make, model, year, license plate, and current mileage.
- Manager can select the vehicle type from a drop-down list
- Manager can select the vehicle's current location from a drop-down list
- Manager can upload a photo of the vehicle
- Manager can add a description of the vehicle
- Manager can save the vehicle

## Vehicle Details

- User can go [Vehicles](#vehicles), or the previous contextual screen
- User can see the vehicle's current status (checked out or available).
- User can see the vehicle's maintenance status, (Overdue, due soon, up-to-date)
- User can see the vehicle's make, model, year, license plate, and current mileage.
- User can see the vehicle's current location.
- User can see the vehicle's photo.
- User can go to the vehicles [Current Trip](#current-trip), if one is in progress.
- User can go to the vehicle's [Trip History](#trip-history)
- User can go the vehicle's [Expenses](#expenses) report
- User can go the vehicle's [Incidents](#incidents) report
- User can add a new maintenance task with the [Maintenance Form](#maintenance-form)
- User can check-in check-out vehicle with a tap.
- Manager can assign the vehicle to a driver with the [Assign Vehicle Form](#assign-vehicle-form)
- User can start a new trip with the [Begin Trip](#begin-trip)
- Manager can edit the vehicle with the [Vehicle Form](#vehicle-form)

## Maintenance

- User can go [Vehicles](#vehicles)
- User can go to [Trips](#trips)
- User can see a list of all maintenance tasks, categorized by overdue, due soon, and up to date.
- User can add a new maintenance task with the [Maintenance Form](#maintenance-form)
- User can edit a maintenance task with the [Maintenance Form](#maintenance-form)
- User can complete a maintenance task
- User can update the status of a maintenance task (in progress, delayed, complete)
- Manager can delete a maintenance task
- Manager can see a list of tasks pending approval (For adding, editing, and changing status)
- Manager can approve or deny a pending request, with an option to comment

## Maintenance Form

- User can cancel, going back to the previous contextual screen.
- User can input the maintenance task's name
- User can input the maintenance task's description
- User can input the maintenance task's due date
- User can input the maintenance task's cost, if known
- User can upload other contextual information
- User can save the task, going back to [Maintenance](#maintenance), or the previous contextual screen.

## Trips

- User can go [Vehicles](#vehicles), or the previous contextual screen
- User can go to [Maintenance](#maintenance)
- User can see their [Current Trip](#current-trip), if one is in progress.
- User can [Begin Trip](#begin-trip) if no trip is in progress.
- User can view [Trip History](#trip-history)

## Begin Trip

- User can cancel, going back to their previous contextual screen.
- User can select the vehicle from the available vehicles.
  - If selected vehicle is not checked out, or the user checked out a different vehicle, the user will be appropriately prompted. Continuing will set the correct vehicle status.
- User can input starting mileage, prepopulated from the previous trip (if any), which the user will confirm is accurate.
- User can start the trip and be redirected to [Current Trip](#current-trip)

## End Trip

- User can cancel, going back to their previous contextual screen.
- User can input ending mileage
- User will confirm that all expenses have been added
  - If not, the user will be redirected to the [Expense Form](#expense-form)
- User will confirm that there are no incidents to report
  - If not, the user will be redirected to the [Incident Form](#incident-form)
- User can confirm to end the trip
- User is asked if they would like to check the vehicle back in, with their response setting the appropriate state
- User is redirected to the [Vehicles](#vehicles) screen

## Trip History

- User can go to [Trips](#trips), or to the previous contextual screen
- Driver can see filterable list of their previous trips
- Manager can see a filterable list of all previous trips
- User can export the list
- User can tap on a trip to view the [Trip Report](#trip-report)

## Trip Report
- User can see trip date and time
- User can see trip driver
- User can see trip vehicle (tapping leads to [Vehicle Details](#vehicle-details))
- User can see used mileage
- User can view [Expenses](#expenses) screen (if any)
- User can view the [Incidents](#incidents) screen (if any)

## Expenses

- User can go back to the previous contextual screen
- User can see a list of all expenses, categorized by maintenance, repair, fuel, and other.
- User go to the [Expense](#expense) report
- User can add a new expense with the [Expense Form](#expense-form)
- User can edit an expense with the [Expense Form](#expense-form)

## Expense

- User should see the type of expense: maintenance, repair, fuel, other
- User should be able to see the receipt of the expense
- User should be able to see shop information, if applicable
- User should be able to see optional driver comments, if applicable

## Incidents

- User can go back to the previous contextual screen
- User should see the time and date of the incident
- User should see a description of the incident
- User should see involved party information
- User should have the option to upload any other contextual information

## Current Trip

- User can go back to [Trips](#trips), or to the previous contextual menu
- User can see the trip vehicle (tapping leads to [Vehicle Details](#vehicle-details))
- User should be able to add an expense with a [Expense Form](#expense-form)
- User should be able to add an incident with a [Incident Form](#incident-form)
- User should be able to end the trip with a [End Trip](#end-trip)

## Incident Form

- User can cancel, going back to the previous contextual screen.
- User can input the time and date of the incident
- User can input a description of the incident
- User can input involved party information
- User can upload any other contextual information
- User can save the incident, going back to the previous contextual screen.

## Expense Form

- User can cancel, going back to the previous contextual screen.
- User can input the type of expense: maintenance, repair, fuel, other
- User can input the cost of the expense
- User can scan the receipt
  - Option to scan the receipt with the [Scanner](#scanner) screen.
  - Option to upload the receipt from the device
- User can input the shop information, if applicable
- User can input optional driver comments
- User can save the expense, going back to the previous contextual screen.

## Scanner

- User can cancel, going back to the previous contextual screen
- User can take a photo of the receipt
- User can upload an existing photo of the receipt
- User can crop the photo
- User can save the photo, going back to the [Expense Form](#expense-form)
