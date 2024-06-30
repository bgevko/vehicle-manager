## Login

- User can log in
- User can register
- User can reset their password

## Vehicles

- User see the list of all vehicles, with available and checked out vehicles grouped separately.
  - Filterable by vehicle type, last driven, last driver, mileage, and maintenance status.
  - Maintenance status includes overdue, due soon, and up to date.
- User can go to [Vehicle Details](#vehicle-details) by selecting a vehicle.
- User can go to the [Trips](#trips) screen
- User can go to the [Maintenance](#maintenance) screen
- Driver can check out or check in a vehicle
- Driver can see their checked out vehicle, along with the information above.
- Manager can assign a vehicle to a driver using the [Assign Vehicle Form](#assign-vehicle-form)
- Manager can unassign a vehicle from a driver
- Manager can go to the [Manage Vehicles](#manage-vehicles) screen

## Assign Vehicle Form

- Manager can select a driver from a drop-down list of available drivers
- Manager can select a vehicle from a drop-down list of available vehicles
- Manager can confirm the assignment
- Manager can cancel the assignment
- Manager can go back to [Vehicles](#vehicles)

## Manage Vehicles

- Manager can add a new vehicle with the [Vehicle Form](#vehicle-form)
- Manager can edit a vehicle with the [Vehicle Form](#vehicle-form)
- Manager can delete a vehicle with a prompt asking if they are sure
- Manager can go back to [Vehicles](#vehicles)
- Manager can go to [Vehicle Details](#vehicle-details)

## Vehicle Details

- User can see the vehicle's current status (checked out or available).
- User can see the vehicle's maintenance status.
- User can see the vehicle's make, model, year, license plate, and current mileage.
- User can see the vehicle's current location.
- User can go to the vehicles [Current Trip](#current-trip), if one is in progress.
- User can go to the vehicle's [Trip History](#trip-history)
- User can go the vehicle's [Expenses](#expenses) report
- User can go the vehicle's [Incidents](#incidents) report
- User can add a new maintenance task with the [Maintenance Form](#add-maintenance-form)
- Driver can check out the vehicle
- Driver can start a new trip with the [Begin Trips Form](#begin-trips-form)
- Manager can assign the vehicle to a driver with the [Assign Vehicle Form](#assign-vehicle-form)
- Manager can edit the vehicle with the [Vehicle Form](#edit-vehicle-form)

## Maintenance

- User can see a list of all maintenance tasks, categorized by overdue, due soon, and up to date.
- User can add a new maintenance task with the [Maintenance Form](#add-maintenance-form)
- User can edit a maintenance task with the [Maintenance Form](#edit-maintenance-form)
- User can complete a maintenance task
- User can update the status of a maintenance task (in progress, delayed, complete)
- Manager can delete a maintenance task with a prompt asking if they are sure
- Manager can see a list of tasks pending approval (For adding, editing, and change the status of a task)
- Manager can approve or deny a maintenance task

## Trips

- The driver can see their current trip, if one is in progress.
- The driver can go to [Current Trip](#current-trip)
- Driver can start a new trip, triggering a [Begin Trips Form](#begin-trips-form) this option is not possible if a trip is already in progress.
- Driver can view [Trip History](#trip-history)

## Begin Trips Form

- The driver can cancel, with a prompt asking if they want to cancel
- The current vehicle. This is pre-filled if the vehicle is already checked out. If not checked out,
  the driver will select the vehicle they want from a drop-down, and it will automatically be checked
  out when the trip starts.
- The driver can input starting mileage, which is pre-populated from the previous trip record, but the driver will verify accuracy.
- The driver can confirm to start the trip

## Trip History

- The driver can go back to [My Trips](#my-trips)
- The driver can see a table of previous trips.
- The driver can export the report as a whole
- The driver can view [Trip Report](#trip-report) screen

## Trip Report

- The user can see used mileage
- The user can see a list of all expenses
- The user can view [Expenses](#expenses) screen
- The user can view the [Incidents](#incidents) screen

## Expenses

- The user can see a list of all expenses, categorized by maintenance, repair, fuel, and other.
- User go to the [Expense](#expense) report
- The user can add a new expense with the [Expense Form](#add-expense-form)
- The manager can edit an expense with the [Expense Form](#edit-expense-form)

## Expense

- The user should see the type of expense: maintenance, repair, fuel, other
- The user should be able to see the receipt of the expense
- The user should be able to see shop information, if applicable
- The user should be able to see optional driver comments, if applicable

## Incidents

- The user should see the time and date of the incident
- The user should see a description of the incident
- The user should see involved party information
- The user should have the option to upload any other contextual information

## Current Trip

- The driver can go back to [My Trips](#my-trips)
- The driver should be able to add an expense with a [Add Expense Form](#add-expense-form)
- The driver should be able to add an incident with a [Add Incident Form](#add-incident-form)
- The driver should be able to end the trip with a [End Trip Form](#end-trip-form)
