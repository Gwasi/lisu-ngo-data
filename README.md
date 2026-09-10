# Lisu Language Dictionary Data

English-Lisu translation dictionary data for the Lisu Ngo project.

## Format

The dictionary is stored as a CSV file with 3 columns:

| Column | Required | Description |
|--------|----------|-------------|
| **English** | Yes | English word or phrase |
| **Lisu** | Yes | Lisu translation |
| **When/Why** | No | Grammar rules, usage notes, or context |

## How to Add or Update Entries

### Basic Entry (no usage notes)

```csv
"hello","ꓧꓪꓸ ꓧꓪꓸ"ꓼ
```

### Entry with Usage Notes (When/Why)

```csv
"and","ꓢꓲ ꓠꓬꓲ꓾", "uses when: go and see, come and go, eating and watching"
```

The **When/Why** column explains **when to use** a word or **why** a translation varies. This helps the AI translator pick the correct Lisu word in different contexts.

### Examples of When/Why Notes

```csv
"called","ꓘꓴ ꓗꓷ" "I called his phone, I called him"
"called","ꓟꓬꓱꓺ ꓖꓶ" "He is called John"
"a (fruit)","(fruit) ꓕꓲꓽ ꓢꓶ", "uses for round objects, eggs and fruits"
"with","ꓐꓰ", "usage: 'with' acts as 'together', do something together"
```

### Rules

1. **Always wrap fields in quotes** if they contain commas, quotes, or special characters
2. **When/Why is optional** — leave it empty if no special context is needed
3. **Be concise** — keep usage notes short and clear
4. **Use parentheses** for variables: `(noun)`, `(verb)`, `(pronoun)`
5. **Use asterisks** for examples: `I called his phone`

### Adding a New Entry

1. Open `default_data.csv`
2. Add a new line at the end (or in alphabetical order)
3. Follow the format: `"English","Lisu","When/Why (optional)"`
4. Commit and push your changes

### Modifying an Existing Entry

1. Find the entry you want to change
2. Edit the English, Lisu, or When/Why column
3. Commit and push your changes

## Contributing

1. Fork this repository
2. Create a branch: `git checkout -b add-new-words`
3. Make your changes to `default_data.csv`
4. Commit: `git commit -m "feat: add new Lisu words"`
5. Push: `git push origin add-new-words`
6. Open a Pull Request

## Usage

This data is used by the Lisu NGO AI Translator application to provide translations between English and the Lisu language.
