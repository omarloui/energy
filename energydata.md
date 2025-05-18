Data Pattern – Cyprus Energy Timeframe Classification
Version 1.1 (supersedes v1.0)

Purpose
Provide training data for a classifier that, given a natural-language question about a smart home’s energy use or solar generation in Cyprus, predicts the time horizon the user cares about.
The model must output exactly one of the six labels:

sql
Copy
Edit
1 hour | 3 hour | 8 hours | 1 week | 1 month | season
Schema
Field	Type	Description
question	string	A user-phrased query about energy consumption, solar generation, costs, or efficiency for a Cyprus smart home.
label	string	Enum: 1 hour, 3 hour, 8 hours, 1 week, 1 month, season  ← the correct timeframe class.

Required
question

label

Example Record
yaml
Copy
Edit
question: "How much energy will my HVAC draw during tonight’s eight-hour sleep schedule?"
label: "8 hours"
