Generates stratified test-train splits for multi-label data.

Example use:

```python
# Import stratified_train_test_split
import sys
sys.path.append('/absolute/path/to/multilabel_stratify')
from stratify import stratified_train_test_split

# Example Data
X = [1,2,3,4,5,6,7,8,9,10]
y = [
    ['prime', 'odd'],
    ['even', 'favourite'],
    ['prime', 'odd'],
    ['even'],
    ['prime', 'odd'],
    ['even'],
    ['prime', 'odd'],
    ['even'],
    ['odd'],
    ['even']
]

# Get the splits
X_train, X_test, y_train, y_test = stratified_train_test_split(
    X, 
    y, 
    target_test_size=0.2, 
    random_state=42)
```

