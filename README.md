# Promptly Template Library

A searchable template library for AI prompts with Fuse.js integration.

## Features
- Searchable template database
- Fast fuzzy search using Fuse.js
- Responsive design
- Easy to customize
- Simple API for mobile applications

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

## API Endpoints
Simple API endpoints are available through [api.html](https://dayanleksonoputro.github.io/Promptly_template/api.html):

### List All Templates
GET [api.html?action=list](https://dayanleksonoputro.github.io/Promtly_template/api.html?action=list)

Returns all templates in JSON format.

### Get Template by ID
GET api.html?action=get&id={template_id}
Returns a specific template by its ID.

### Search Templates
GET api.html?action=search&q={search_term}
Returns templates matching the search term using fuzzy search.

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
5. Your site will be available at [https://dayanleksonoputro.github.io/Promtly_template/](https://dayanleksonoputro.github.io/Promtly_template/)

These changes will allow your Android application to consume your template data through simple HTTP requests:
- To get all templates: https://yourusername.github.io/Promptly_template/api.html?action=list
- To get a specific template: https://yourusername.github.io/Promptly_template/api.html?action=get&id=template_1
- To search templates: https://yourusername.github.io/Promptly_template/api.html?action=search&q=lesson
The API responses will be in JSON format that your Android app can easily parse. This approach works with GitHub Pages since it's still serving static files, but provides the API-like functionality your Android app needs.
