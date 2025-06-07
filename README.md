# Notion Transformer

A tool to transform Notion API page properties into a cleaner format.

## Installation

```bash
pip install notion_transformer
```


## Usage

```bash
notion_transformer input.json
```

This will print the transformed properties to the console.

You can also use it as a library:

```python
from notion_transformer import transform_notion_properties
import json

with open("input.json", "r") as f:
    data = json.load(f)
    properties = data["properties"]  # Assuming the input JSON has a 'properties' key
    transformed_properties = transform_notion_properties(properties)
    print(transformed_properties)
```


