# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  class User{
        - name: string
        - email: string
        - password: string
        - typingTests: vector~test~
        + login(user: string, pass: string) boolean
        + get_email() string
        + get_tests() vector~test~
  }
  class test{
        - id: string
        - phrase: string
        - user_input: string
        - accuraryPercentage: int
        - wpm: float
        + add_test(phrase: string, user_input: string, time: float)
        + get_accurary() int
        + calc_wpm() float
  }
```
