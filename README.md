# SimpleLogger
Simple logger mainly for monitoring learning.


# Example
```python
from logger import SimpleLogger as Logger


logger = Logger("loss", "accuracy")

for epoch in range(10):
  loss = 11.2
  acc = 0.4
  logger.append("loss", loss)
  logger.append("accuracy", acc)

  logger.save("epoch_{}".format(epoch))

```
