# kaspersky passwords manager export to csv passwords manager

## Instructions:

### Export your kaspersky passowords.
1. Enter the [official docs](https://support.kaspersky.com/help/KPM/Win24.0/en-US/130515.htm)
2. Follow the instructions in `Export data in printable format from My Kaspersky`

### Convert it to CSV
```python
python3 convert.py dd-mm-yyyy.txt
```

## Limitations

### Different Interface
Kaspersky and google passwords managers do not share the same interface, google is more limited.
Kaspersky passwords manager supports:
- websites
- apps
- notes
- credit cards
- documents
- adresses
Google passwords manager supports only:
- websites
Because of that, the code takes from kaspersky only the websites and apps and saves them all in googles websites format.
