```mermaid
flowchart TD
    A[Oh no, my assignment is due!] --> B(Time to make a diagram with Mermaid)
    B --> C{What should I make?}
    C -->|I want an easy to document system| D[A sequence diagram of user-input validation]
    C -->|I **need** at least four entities| E[A state diagram of the writing process]
    D -->|I only made three entities and don't know how to expand!| F(I know now.)
    E -->|Documenting every relation is going to take forever!| F
    F -->G(A flowchart of my decision process while creating it.)
```

# Entities
## __Oh no, my assignment is due!__
This represents 11 A.M. September 29th, when I realized I had an assignment due.
## __Time to make a diagram with Mermaid__
I had skimmed the Mermaid Documentation earlier, but only actual read it on the day it was due.
## __What should I make?__
I checked the diagram types and tried to come up with modelable scenarios.
## A sequence diagram of user-input validation
This was something that I had a lot of experience with, both using and developing.
```mermaid
sequenceDiagram
    actor U as User
    participant C as Client
    participant S as Server
    Note left of U: Let's try an answer
    U->>C: Answer
    Note right of C: Answer is hashed
    C->>S: Request for URL containing hash
    alt 200 Response
        S->>C: Data
        C->>U: Content
        Note left of U: Hooray, I solved!
    else 4xx Response
        S-->>C: Lack of Data
        C-->>U: Error Message / Lack of Content
        Note left of U: Aw man, I better try something else
    end
```
###### The completed diagram
## A state diagram of the writing process
I thought it would be a nice thing to model, but realized the complexity was much greater than my current skill.
## I know now.
With both of my current options seemingly nonviable, I came up with another.
## A flowchart of my decision process while creating it.
This is said flowchart.

# Relations
The labels on either side show the reasoning behind each decision.
This diagram isn't __entirely__ accurate, as the attempt at a state diagram was directly influenced by the sequence diagram. However, the thought process could have essentially gone the other way, as was thus bifurcated.
