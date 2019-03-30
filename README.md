### mamba
---
https://nestorsalceda.com/mamba/

```py
from mamba import description, context, it
from expects import expect, equal

with description() as self:
  with it():
    rafa_nadal = ""
    roger_federer = ""
    game = Game(rafa_nada, roger_federer)
    
    expect(game.score()).to(equal((0, 0)))
    
    











# tennis_spec.py
from mamba import description, context, it
from expects import expect, equal

import tennis

with description('Tennis') as self:
  with it('starts with 0 - 0 score'):
    rafa_nadal = "Rafa Nadal"
    roger_federer = "Roger Federer"
    game = tennis.Game(rafa_nadal, roger_federer)
    
    expect(game.score()).to(equal((0,0)))


class Game(object):
  def __init__(self, player1, player2):
    pass
    
  def score(self):
    return (0, 0)
```

```
pipenv install mamba
pip install mamba

pipenv run mamba tennis_spec.py
```

```
```


