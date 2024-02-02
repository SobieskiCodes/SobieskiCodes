![Header image](https://raw.githubusercontent.com/SobieskiCodes/SobieskiCodes/main/Assets/GitHub_Header.jpg)



[comment]: <> (https://www.freepik.com/search?format=search&query=technology&type=icon hello future me)
Hi there, I'm Justin 👋
<img align='right' src="https://raw.githubusercontent.com/SobieskiCodes/SobieskiCodes/main/Assets/SideImageDown.png">


```python

from dataclasses import dataclass, field
from typing import List, Dict, Union


def create_field(values: Union[list[str], dict]):
    return field(default_factory=lambda: values)


@dataclass
class Person:
    name: str = 'justin'
    age: int = 32
    email: str = 'jmksobieski@gmail.com'
    discord: str = 'probsdad'
    pronouns: List = create_field(["him", "he"])
    code: List = create_field(["Javascript", "HTML", "React", "Python", "PHP"])
    technologyInterests: List = create_field(["Automation", "APIs", "OSCP", "Kernal Injection"])
    pursuing: str = 'Bachelor of Science in Computer Science'
    currentWork: str = 'Support Engineer'
    goals: Dict = create_field({"collect": "the fish", "youToRunThis": f'mailto:?to='})

    def contact(self):
        response = f"You can contact me by email at, " \
                   f"{self.goals.get('youToRunThis')}{self.email} " \
                   f"or discord at {self.discord}."
        return response


me = Person()
print(me.contact())


```

<p align="center" width="100%">
    <img width="33%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SobieskiCodes&theme=radical&show_icons=true&layout=compact"> 
</p>

