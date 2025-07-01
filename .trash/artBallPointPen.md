---
promptId: 'artBallPointPen'
name: '🖼️ Generate a ball-point pen photo'
description: 'select a text and photo with the style of ball-point pen will be generated using Dalle-2'
author: 'Prompt Engineering Guide'
tags: 'photo, dalle-2, art'
version: '0.0.1'
output: '\n![]({{requestResults.data.0.url}})'
provider: 'custom'
endpoint: 'https://api.openai.com/v1/images/generations'
body: '{"n": 1, "size": "1024x1024", "prompt": "{{escp prompt}}"}'
---
{{selection}}, ball-point pen art