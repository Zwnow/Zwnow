- 👋 Hi, I’m @Zwnow
- 👀 I’m interested in learning new stuffs and things!
- 🌱 I’m currently learning development in ERP systems (currently in apprenticeship and working with Dynamics).
- 📫 How to reach me svenotimm@gmail.com




class Labyrinth(object):
    def __init__(self, width, height):
        self.labyrinth = """XSXXXXXXXXX0000XXXXXXXXX0XXXXXXXXX00000XXXXXXXXXFX"""
        self.width = width
        self.height = height

    def PrintLabyrinth(self):
        #Starting values
        width1 = 0
        width2 = self.width
        #Formula and printing
        for rows in range(self.height):
            width1 = rows*self.width
            width2 = (rows+1)*self.width
            print(self.labyrinth[width1:width2:1])

    def GetPosition(self):
        return self.labyrinth.index("S")
    
    def CheckNextStep(self):
        position = self.GetPosition()
        print(position)

lab = Labyrinth(10,5)

lab.CheckNextStep()


<!---
Zwnow/Zwnow is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
