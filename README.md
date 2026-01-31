# cognitive-angles-dataset
Multi-perspective fairy tales for AI training and cognitive science research
# Cognitive Angles Dataset

## Overview
A multi-modal dataset for testing and training multi-perspective reasoning in AI systems. Contains 38+ annotated literary narratives ("crooked fairy tales") encoding 17 distinct cognitive perspectives.

## Structure
- `/data/fairy_tales/` - Annotated narratives in JSON format
- `/data/phenomena/` - 500+ cognitive phenomena with formal grammar
- `/evaluation/` - Scripts for angle detection and analysis
- `/paper/` - Research paper and documentation
- `/multimodal/` - Illustrations and supplementary materials

## Cognitive Angles
1. Naive, 2. Linguistic, 3. Absurd, 4. Philosophical, 5. Metaphorical, 
6. Introspective, 7. Ironical, 8. Grotesque, 9. Socio-critical, 
10. Poetic, 11. Communal, 12. Capitalist-critical, 13. Ontological,
14. Auditory, 15. Performative, 16. Surreal, 17. Literal

## Quick Start
```python
import json

# Load a sample fairy tale
with open('data/fairy_tales/001_mys.json', 'r') as f:
    tale = json.load(f)
    
print(f"Title: {tale['title']}")
print(f"Primary angle: {tale['cognitive_analysis']['primary_angles'][0]}")
