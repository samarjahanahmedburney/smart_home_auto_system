# smart_home_auto_system
this is smart home automation system its allow user to control and monitor various home appliances using python data structures like LIST,TUPLE,DICTIONARIES,SETS AND FUNCTIONS.

print("Task 1.1: Device Management (Lists & Tuples)\n")

# Initial list of smart devices
devices = ["Light" , "Fan" , "AC" , "Doorlock" , "Thermostat"]
print(devices)
print()

# Add a new device
new_devices = input(("Add a New Device: "))
devices.append(new_devices)
print(devices)
print("New Device:" , new_devices )
print()

# Remove a device
remove_devices = input(("Remove Device: "))
devices.remove(remove_devices)
print(devices)
print("Removed Device:" , remove_devices )
print()

# Sort devices alphabetically
devices.sort()
print("Sorted Devices:" , devices)
print()

print("Task 1.2: Store Device Settings Using Tuples")

# Define device tuple.
lights = ("Lights" , "ON" , 60 )
Fan = ("Fan" , "OFF" , 40 )
AC= ("AC" , "ON" , 1500 )

# store all device in a list.
devices = [lights , Fan , AC]

# Show all device with status and power.
for device in devices:
    print(f" {device[0]}: Status = {device[1]}, Power = {device[2]} Watts")
print()

print("Task 2.1: Energy Consumption Tracker (Dictionaries & Sets)\n")
# Initize energy usage in a Dictonary
energy_usage = {
    "Lights": 5,
     "AC": 120,
    "Fans": 30
   }

# Show Initial usage
print(f"Initial Energy Usage: {energy_usage}")

# Add new device.
energy_usage['Thermostat'] = 20

# Update a device
energy_usage['AC'] = 110
print(f"Updated Energy Usage: {energy_usage}")

# Remove a device (e.g remove Refrigerator )
# energy_usage.pop('Refrigerator')

# Total energy consumption.
energy_usage_total = sum(energy_usage.values())
print(f"Total Energy Consumption: {energy_usage_total} Watts")
print()

print("Task 2.2: Identify Unique Power-Saving Modes Using Sets\n")

# Initize power saving mode.
power_modes = {'Eco Mode', 'Night Mode'}
print( "Power Saving Modes: ", power_modes)

# Add a new mode.
new_mode = "Away Mode"
power_modes.add(new_mode)
print(f"New Mode Added: '{new_mode}' ")

# View all power-saving modes
print("Updated Modes: ", power_modes)
print()

# Check if a mode is available.
check_mode = "Away Mode"
if check_mode in power_modes:
    print(f"{'Away Mode'}, is available.")
else:
    print(f"{'Away Mode'}, is not available.")
print()

print("3.1: Functions for Smart Home Automation Task\n")

# don't use function topic

# Take input from the User
energy_usage = float(input(" Enter Total energy usage in (kWh): "))
rate_per_kwh = float(input(" Enter Electricity rate per kWh (in $): "))

# Total cost calculate
total_cost = energy_usage * rate_per_kwh

# Display the total monthly energy cost.
print(f" Total Monthly Energy Cost: ${total_cost:.2f}")
print()

print("Task 3.2: Create a Function to Find Common Devices in Two Homes\n")

# don't use function topic

# List of devices in Two homes
home1_devices = ['Lights' , 'AC' , 'Fan']
home2_devices = ['Lights' , 'Door Locks' , 'Fan']

# Convert list to set
set1 = set(home1_devices)
set2 = set(home2_devices)

# Find common devices
common_devices = set1 & set2

# Display output
print(f"Common Devices : {common_devices}")

print("Task 4.1: Create an Automation Rule Using Functions\n")

# don't use function topic

device = 'Lights'
time = "10:00 PM"
action = "OFF"

print(f" Automation Rule: {device} will be turned {action} at {time}.")
print()

print("Task 4.2: Function to Optimize Power Consumption\n")

devices = [("Lights", 60), ("AC", 1500), ("Fan", 40), ("Heater",2000)]
active_devices = []

# name = devices[0]
# power_usage = devices[1]

for device in devices:
  name = device[0]
  power = device[1]
  if power<=1000:
    active_devices.append(name)
print(active_devices)
print()

print("Bonus Challenge:\n")

name = "Alice"
device1 = "lights"
device2 = "AC"
status1 = "off"
status2 = "on"
print(f"Checking status for: {device1} , {device2}")
print(f"{device1.capitalize()} set to {status1.upper()}")
print(f"{device2.capitalize()} set to {status2.upper()}")
print()

