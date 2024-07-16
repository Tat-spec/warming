# warmingclass ClimateModel:
    def __init__(self, initial_temperature):
        self.temperature = initial_temperature

    def increase_temperature(self, factor):
        self.temperature *= factor

    def decrease_temperature(self, factor):
        self.temperature /= factor

# Example usage:
climate = ClimateModel(initial_temperature=15.0)

# Simulating temperature changes
print(f"Initial temperature: {climate.temperature} °C")

# Increase temperature due to greenhouse gases
climate.increase_temperature(factor=1.2)
print(f"Temperature after greenhouse effect: {climate.temperature} °C")

# Decrease temperature due to natural factors or mitigation efforts
climate.decrease_temperature(factor=1.5)
print(f"Temperature after natural cooling or mitigation: {climate.temperature} °C")
