# Tureng Dictionary - API Guide

## Overview
Python wrapper for the Tureng Turkish-English dictionary database.

## Quick Start
```python
from tureng import Tureng

t = Tureng()
results = t.translate("merhaba")
for r in results:
    print(f"{r.turkish} -> {r.english}")
```

## Features
| Feature | Description |
|---------|-------------|
| Word Lookup | Turkish to English translation |
| Reverse Lookup | English to Turkish |
| Multiple Meanings | All definitions returned |
| Categories | General, slang, idioms, etc. |

## Response Format
| Field | Type | Description |
|-------|------|-------------|
| turkish | string | Turkish word/phrase |
| english | string | English translation |
| category | string | Usage category |
| type | string | Part of speech |