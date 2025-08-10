# Instructions for Gemini

This document outlines the process for generating content for the Bilingual Parenting project.

## Project Concept

The goal of this project is to create a collection of CSV files containing English words and phrases for parents. These files are designed to help parents incorporate English into their daily interactions with their children, with content tailored to specific age groups from 0 to 10 years old.

## Directory Structure

A single `data` directory will be used to store all CSV files.

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

The content for the `text` column should be relevant to the specified age group and can include the following themes, categorized by developmental stage:

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
