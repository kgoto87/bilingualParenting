# Instructions for Gemini

This document outlines the process for generating content for the Bilingual Parenting project.

## Content Generation Process

The content generation is a two-step process:

1.  Create a JSON file containing the themes for the year.
2.  Generate a CSV file for the year based on the themes in the JSON file.

---

## Step 1: Generate a JSON file of themes

The first step is to create a JSON file that lists the themes for a given year. This file will serve as the source for the CSV file generation.

### JSON File Naming Convention

The JSON file should be named using the following format: `themes-{year}.json`.

For example:

-   `data/themes-2025.json`

### JSON File Structure

The JSON file should be an array of objects, where each object represents a theme and has the following structure:

```json
{
    "ageGroup": "Toddler",
    "category": "item",
    "wordOrPhrase": "milk"
}
```

-   `ageGroup`: The target age group (e.g., "Baby", "Toddler", "Preschooler").
-   `category`: The category of the theme (e.g., "item", "action", "milestone").
-   `wordOrPhrase`: The specific word or phrase for the theme.

---

## Step 2: Generate the CSV file from the JSON file

Using the generated `themes-{year}.json` file, create a CSV file with the content for the year.

## Directory Structure

A single `data` directory will be used to store all CSV and JSON files.

## File Naming Convention

The CSV files will be named by year.

For example:

-   `data/2025.csv`
-   `data/2026.csv`

## CSV File Structure

Each row in the CSV file must contain two columns:

1.  **datetime**: The date and time when the text is intended to be posted, in `YYYY/MM/DD HH:MM` format (e.g., `2025/09/30 07:45`).
2.  **text**: The English word or phrase.

The CSV MUST NOT contain a header row.

## Posting Frequency

Content should be generated for posting three times a day. The `datetime` in the CSV should reflect this, with distinct times for each age group:

-   **Morning (7am):** Babies (0-1 year)
-   **Afternoon (12pm):** Toddlers (1-3 years)
-   **Evening (5pm):** Preschoolers (3-5 years)

## Text Structure

The `text` column should follow this structure:

```
{emoji}{word or phrase}{emoji}

{example No. 1 in daily conversation}

{example No.2 if the first example is too short}
```

For example:

```
🍼Milk🍼

"It's time for your milk!"
"Would you like to hold the milk bottle yourself?"
```

The total content must be less than 140 characters to be compatible with X (formerly Twitter).

### Content Themes for "text" Column

The content for the `text` column should be relevant to the specified age group and can include the following themes, categorized by developmental stage. To ensure a variety of content, themes should not be duplicated within the same CSV file or the same year.

#### Babies (0-1 year)

-   **Baby-Specific Items**: "nappies," "baby wipes," "dummies," "pacifier," "crib," "stroller," "formula," "bib."
-   **Actions and Milestones**: "crawling," "tummy time," "babbling," "clapping hands," "peek-a-boo."
-   **Parental Interactions**: "Are you hungry?", "Let's change your nappy," "Time for a nap," "Look at the light!"

#### Toddlers (1-3 years)

-   **Actions and Milestones**: "first steps," "running," "climbing," "potty training," "stacking blocks."
-   **Daily Objects**: "sippy cup," "plate," "spoon," "pajamas," "potty."
-   **Parental Instructions**: "Hold my hand," "Let's put on your shoes," "Time to clean up your toys," "Can you say 'thank you'?"

#### Preschoolers (3-5 years)

-   **Actions and Milestones**: "pretend play," "drawing," "riding a tricycle," "learning ABCs," "counting."
-   **Daily Objects**: "crayons," "books," "puzzles," "lunchbox," "backpack."
-   **Parental Instructions**: "Let's read a story," "What color is this?", "Share your toys with your friend," "Use your words, please."
