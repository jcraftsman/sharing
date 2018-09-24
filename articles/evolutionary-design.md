# Real world Evolutionary Design

## Agenda

Code and discussion

The first iteration is about micro design.
We will implement a requirement following a set of rules and constraints.
Then we will take a brief retrospective look about our designs and try to understand how these rules have impacted it.

The second iteration is about macro design.
We will refactor a working implementation (The code we will refactor has been written following the same rules of iteration 1).
We will take a step back and look to our designs and try to identify the weaknesses and the strengths.

Finally, we will conclude by a quick presentation about Evolutionary Design.

## Design Decisions made during this workshop

Be aware of the biais
Using a class
Areas of Volatility:

- OCR
- File Finder? always access to the filesystem?

## Deductive approach

- Acceptance test guide the implementation.
- Acceptance test probe the behavior
- Unit tests probe the design
- Unit tests are coupled with design decisions
- Almost each unit test reprensents a design decision

- Design in Red can be tricky (solution biais)
- It constraints discovery

- Mocking is keeping us isolated
- Mocks are coupled to the structure
- Domain is only to satisfy requirements
- All methods are created to satisfy a client

- Use my experience and what I have learned in the past

## Inductive approach

- Works well for exploration
- Speculative development

## Evolutionary Design

- Design is part of coding
- As the code evolves the design changes

- Changing requirements => Design for flexibility
- What changes are you expecting?
- It's hard to identify (Misunderstanding the problem / Changing business): Some changes are due to misunderstanding the requirements or the problem. But most important changes can be related to the change on the business itself.

- Evolutionary Design is not about code and fix.

- Value simplicity:
- Do the simplest thing that could possibly work
- And try to find the balance between what YAGNI (You aren't gonna need it) and Flexible design

- Rules of simple design:
1. Passes the tests
2. Reveals intention (Easy to understand. Relative: Team members should be familiar with design concepts)
3. No duplication (Beware of accidental duplication: Removing accidental duplication may lead to accidental complexity and break flexibility)
4. Fewest elements

- Keep the code clear and simple
- You won't get the simplest design at the first shot
- Don't worry, at the end, you can and you should refactor
- Today's decisions will have to be changed tomorrow
- Communicate the design to the people who needs to understand it

Evolutionary design doesn't like frameworks
Grows organicaly vs within a frame.
Try to solve a problem vs Fit your solution within a frame.
Prefer use libraries (in isolation for generic subdomains)

