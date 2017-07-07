This Dockerfile allows to play with [Polyglot](https://github.com/aboSamoor/polyglot), a natural language pipeline with multilingual support.

Install Docker, and run the following commands:

```
docker pull 0asa/polyglot-docker
docker run -ti 0asa/polyglot-docker python
```

You'll end up in a Python interpreter where you can play with polyglot awesomeness:

```py
import polyglot
from polyglot.text import Text, Word
text = Text("Hello, my name is Vincent")
for ent in text.entities:
    print(ent.tag, ent)
```
