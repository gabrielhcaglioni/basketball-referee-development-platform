# System Entities

## Referee

Represents a basketball referee.

Attributes:

- id
- name
- category
- federation
- region
- years_of_experience

---

## Game

Represents a game worked by referees.

Attributes:

- id
- date
- competition
- category
- home_team
- away_team

---

## Self Assessment

Represents the referee's perception after a game.

Attributes:

- id
- referee_id
- game_id
- overall_perception
- strongest_point
- main_difficulty
- external_factors
- comments

---

## Coordinator

Represents an evaluator or coordinator.

Attributes:

- id
- name
- role

---

## Observation

Represents a development observation.

Attributes:

- id
- coordinator_id
- referee_id
- game_id
- category
- subcategory
- description

---

## Feedback Session

Represents the post-game meeting.

Attributes:

- id
- game_id
- coordinator_id
- summary
- development_points
