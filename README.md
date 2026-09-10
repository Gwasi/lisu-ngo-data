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
"hello","ꓧꓪꓸ ꓧꓪꓸ"
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

## Editing on GitHub (No Software Required)

You can edit the dictionary directly on GitHub's website — no installation needed.

### Step 1: Create a GitHub Account

1. Go to [https://github.com](https://github.com)
2. Click **Sign up**
3. Enter your email, create a password, and choose a username
4. Verify your email address

### Step 2: Sign In

1. Go to [https://github.com/login](https://github.com/login)
2. Enter your username/email and password
3. Click **Sign in**

### Step 3: Fork the Repository

1. Go to [https://github.com/Gwasi/lisu-ngo-data](https://github.com/Gwasi/lisu-ngo-data)
2. Click **Fork** (top right corner)
3. Click **Create fork** — this creates your own copy

### Step 4: Edit the CSV File

1. In your forked repository, click on `default_data.csv`
2. Click the **pencil icon** (Edit this file) in the top right
3. Make your changes to the CSV
4. Scroll down to the **Commit changes** section
5. Add a short description (e.g., "Add new word: hello")
6. Click **Commit changes**

### Step 5: Submit a Pull Request (to share your changes)

1. Go back to your forked repository
2. Click **Contribute** → **Open pull request**
3. Add a description of what you changed
4. Click **Create pull request**

Your changes will be reviewed and merged into the main dictionary.

### Quick Reference: CSV Format

Each line follows this format:
```csv
"English","Lisu","When/Why (optional)"
```

Example:
```csv
"hello","ꓮ ꓡꓯꓼ","usage: greeting"
```

## Usage

This data is used by the Lisu NGO AI Translator application to provide translations between English and the Lisu language.
