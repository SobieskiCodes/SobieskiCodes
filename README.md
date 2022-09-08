### Hi there, I'm Justin 👋
![Header image](https://raw.githubusercontent.com/SobieskiCodes/SobieskiCodes/main/Assets/GitHub_Header.jpg)



[comment]: <> (https://www.freepik.com/search?format=search&query=technology&type=icon hello future me)

<img align='right' src="https://raw.githubusercontent.com/SobieskiCodes/SobieskiCodes/main/Assets/SideImage.png">



```python
from dataclasses import dataclass, field
from typing import List, Dict


@dataclass
class Person:
    name: str = 'justin'
    age: int = 30
    email: str = 'jmksobieski@gmail.com'
    discord: str = 'ProbsJustin#2162'
    pronouns: List = field(default_factory=lambda: ["him", "he"])
    code: List = field(default_factory=lambda: ["Javascript", "HTML", "CSS", "Python", "PHP"])
    technologyInterests: List = field(default_factory=lambda: ["Automation", "APIs", "OSCP", "Kernal Injection"])
    pursuing: str = 'Business Administration in Computer Information Systems'
    currentWork: str = 'Security & Infrastructure in the mortgage sector'
    goals: Dict = field(default_factory=lambda: {"collect": "the fish", "youToRunThis": f'mailto:?to='})

    def __repr__(self):
        return self.email

    def contact(self):
        return f"You can contact me by email, {self.goals.get('youToRunThis')}{self.email} or discord at {self.discord}"


me = Person()
print(me.contact())
```
