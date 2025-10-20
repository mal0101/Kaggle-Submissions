As we go through this, keep in mind that submissions are evaluated using F1 between the predicted and expected answers.

F1 is calculated as follows:

        F1 = 2 * (precision * recall) / (precision + recall)

where:

        precision = (TP) / (TP+FP) && recall = (TP) / (TP+FN)

### Data description

- The text of a tweet
- A keyword from that tweet (could be blank)
- The location the tweet was sent from (could also be blank)

#### Columns

- `id` - a unique identifier for each tweet
- `text` - the text of the tweet
- `location` - the location the tweet was sent from (may be blank)
- `keyword` - a particular keyword from the tweet (may be blank)
- `target` - in **train.csv** only, this denotes whether a tweet is about a real disaster (1) or not (0)

### What to predict
Predict whether a given tweet is about a real disaster or not. If so, predict a 1. if not predict a 0.

