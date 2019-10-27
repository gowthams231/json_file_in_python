#python code

import json
with open('states.json') as f:
  data = json.load(f)
for i in data['states']:del i['abbreviation']
with open('new_states.json','w') as f:
  json.dump(data.f.indent=2)
