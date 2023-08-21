# Python OOPS

## Class object in another class
  ```sh

class Driver:
    def __init__(self, name):
        self.name = name

    def test(self):
        print(self.name)


class Car:
    def __init__(self, cname):
        self.cname = cname

    def testc(self):
        print(self.cname)

    def getDriverDetails(self, d):
        d.test()

  ```
