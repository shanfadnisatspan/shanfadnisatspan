<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>

Hi There, I am Shantanu Fadnis and this is my Arsenal.
    
```python
​
from __future__ import annotations

import json
from dataclasses import asdict, dataclass


@dataclass
class Arsenal:
    languages: tuple[str, ...] = ("Python", "Scala", "Java")
    databases: tuple[str, ...] = ("PostgreSQL", "DynamoDB")
    datawarehouses: tuple[str, ...] = ("Hive", "Glue")
    misc     : tuple[str, ...] = ("Apache Spark", "Docker", "SQS", "SNS")
    ongoing  : tuple[str, ...] = ("Scala - Functional Aspects")

    def jsonify(self) -> str:
        return json.dumps(asdict(self), indent=4)


arsenal = Arsenal()
print(arsenal.jsonify())
​
```
</h3>