# Digital-energy-meter-
Digital Energy Meter is a system used to calculate and display the electrical energy consumed by a device or household. The Python program takes voltage, current, and usage time as input and calculates power and energy consumption.
# Digital Energy Meter

print("===== DIGITAL ENERGY METER =====")

voltage = float(input("Enter voltage (V): "))
current = float(input("Enter current (A): "))
time = float(input("Enter usage time (hours): "))
rate = float(input("Enter electricity rate per kWh: "))

# Calculate power
power = voltage * current

# Calculate energy
energy = (power * time) / 1000

# Calculate cost
cost = energy * rate

print("\n----- Energy Report -----")
print("Voltage:", voltage, "V")
print("Current:", current, "A")
print("Power:", power, "W")
print("Energy Consumed:", energy, "kWh")
print("Electricity Cost: ₹", round(cost, 2))

print("\nEnergy measurement completed.")
