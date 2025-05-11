# Base class
class Superhero:
    def __init__(self, name, power, origin):
        self.name = name
        self.power = power
        self.origin = origin

    def introduce(self):
        print(f"I am {self.name} from {self.origin}. My power is {self.power}.")

    def use_power(self):
        print(f"{self.name} uses {self.power}!")

# Subclass
class FlyingSuperhero(Superhero):
    def __init__(self, name, power, origin, flight_speed):
        super().__init__(name, power, origin)
        self.flight_speed = flight_speed

    def use_power(self):
        print(f"{self.name} soars through the sky at {self.flight_speed} km/h using {self.power}!")

# Creating instances
hero1 = Superhero("ShadowStrike", "Invisibility", "Night City")
hero2 = FlyingSuperhero("SkyBlaze", "Fire Manipulation", "Cloud Realm", 300)

# Demonstrating methods
hero1.introduce()
hero1.use_power()

hero2.introduce()
hero2.use_power()
