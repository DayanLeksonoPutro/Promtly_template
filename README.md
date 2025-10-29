# Promptly Template Library

A searchable template library for AI prompts with Fuse.js integration.

## Features
- Searchable template database
- Fast fuzzy search using Fuse.js
- Responsive design
- Easy to customize

## Templates Included
The template database includes:
- Educational tools (Lesson Plan Generator)
- Developer tools (Code Explainer)
- Marketing tools (Product Description Writer)
- Midwifery resources (Communication, Pregnancy Care, Documentation, Entrepreneurship)
- Anatomy and Physiology guides
- Nutrition and Diet information

## Usage
1. Open [index.html](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html) in a web browser
2. Search for templates using the search box
3. Browse results with name, description, and tags

## Data Structure
Templates in [data.json](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/data.json) include:
- `id`: Unique identifier
- `icon`: Material icon name
- `name`: Template name
- `description`: Brief description
- `systemPrompt`: System prompt for AI
- `tags`: Comma-separated tags
- `responseTone`: Preferred tone
- `temperature`: Creativity level (0.0 to 1.0)
- `maxTokens`: Maximum response length

## Customization
To add new templates:
1. Edit [data.json](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/data.json) with new template objects
2. Refresh [index.html](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html) in browser

## Technologies Used
- [Fuse.js](https://fusejs.io/) for fuzzy search
- Vanilla JavaScript
- HTML/CSS

## Deployment to GitHub Pages
1. Create a new repository on GitHub
2. Push these files to the repository
3. Go to Settings > Pages
4. Select "Deploy from a branch" and choose your main branch
5. Your site will be available at `https://[username].github.io/[repository-name]/`