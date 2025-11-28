# Markdown to PDF Resume Generation Tool

A simple Python script that converts Markdown-formatted resume content into a resume PDF using ReportLab.

## Features

- Easier resume modification
- Sections (##), subsections (###), bullet points (*), and horizontal rules (---)
- Header with name, contact info, and subtitle
- Styling with Times font family

## Prerequisites

- Python
- ReportLab module

## Installation

1. Type: 

```bash
git clone <this_URL>.git
```

2. Install the required dependency:

```bash
pip install reportlab
```

## Usage

1. Create your resume content in Markdown format. Save it as `resume.md` in the same directory as `main.py`. (CAUTION: The program is case sensitive)
2. Customize the header information in `main.py`:
   - Replace `"Name LastName"` with your actual name (line 15)
   - Update the contact info string with your phone, email, and website (line 19)
   - Modify the subtitle to something suitable for your professional direction (line 24)
3. Run the script:

```bash
python main.py
```

4. The generated PDF will be saved as `resume.pdf` in the same directory

## IMPORTANT: Markdown Format Guidelines

Use the following Markdown elements for your resume:

- `## Section Title` - Creates a main section header (e.g., ## Experience, ## Education)
- `---` - Inserts a horizontal rule separator below the main section header (This is a common design choice for resumes)
- `### Subsection Title` - Creates a subsection header within a section
- `* Bullet point text` - Creates a bullet point
- Regular text - Normal paragraph content

Example structure:

```
## EDUCATION
---
B.S. in Something at Somewhere University

## SKILLS
---

### Technical Skills
* TensorFlow/Keras
* Brain computer interface and upper limb prosthetics design
* Web development: JavaScript, HTML/CSS, Svelte5, Supabase
* iOS development (Swift, SwiftUI/UIKit)
* Git, Docker

### Natural Language
* Native proficiency: French, English


## PROJECTS/EXTRACURRICULARS 
---

### Oct 2025 – Now | Co-founder, club name
* redacted bullet point
* redacted bullet point

### Oct 2025 – Now | Co-founder, club name
* redacted bullet point
* redacted bullet point
```

## Troubleshooting

- Ensure your Markdown file is properly formatted and named correctly as `resume.md`
- Check that ReportLab is correctly installed
- Check that `resume.md` is in the same directory
- Sorry for the sloppy features, this was a personal utility script
