class Base:
    def __init__(self):
        print("Inside class Base default constructor")

class Derived(Base):
    def __init__(self, x):
        super().__init__()
        print("Inside class Derived constructor, value is ", x)

if __name__ == "__main__":
    obj = Derived(100)
