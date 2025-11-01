# Promptly Template Library

A searchable template library for AI prompts with Fuse.js integration.

## Features
- Searchable template database
- Fast fuzzy search using Fuse.js
- Responsive design
- Easy to customize
- Simple API for mobile applications

## Templates Included
The template database includes templates across various domains:
- Educational tools (Lesson Plan Generator)
- Developer tools (Code Explainer)
- Marketing tools (Product Description Writer)
- Healthcare and Midwifery resources
- Anatomy and Physiology guides
- Nutrition and Diet information
- Job search and career guidance (including Indonesia-specific resources)
- Academic writing and research tools

## Usage
1. Open [index.html](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html) in a web browser
2. Search for templates using the search box
3. Browse results with name, description, and tags

## Data Structure
Templates in [data.json](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/data.json) include:
- `id`: Unique 4-digit identifier (e.g., "0001")
- `icon`: Material icon name
- `name`: Template name
- `description`: Brief description
- `systemPrompt`: System prompt for AI
- `tags`: Comma-separated tags
- `responseTone`: Preferred tone
- `temperature`: Creativity level (0.0 to 1.0)
- `maxTokens`: Maximum response length

## API Endpoints
Simple API endpoints are available through [index.html](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html):

### List All Templates
GET [index.html?api=true](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html?api=true)

Returns all templates in JSON format.

### Search Templates
GET [index.html?api=true&q={search_term}](file:///Users/dayanleksonoputro/Documents/Appnovasi/Promtly_template/index.html?api=true&q={search_term})

Returns templates matching the search term using fuzzy search.

## Technologies Used
- [Fuse.js](https://fusejs.io/) for fuzzy search
- Vanilla JavaScript
- HTML/CSS

## Deployment to GitHub Pages
1. Create a new repository on GitHub
2. Push these files to the repository
3. Go to Settings > Pages
4. Select "Deploy from a branch" and choose your main branch
5. Your site will be available at [https://yourusername.github.io/your-repo-name/](https://yourusername.github.io/your-repo-name/)

These changes will allow your Android application to consume your template data through simple HTTP requests:
- To get all templates: https://yourusername.github.io/your-repo-name/index.html?api=true
- To search templates: https://yourusername.github.io/your-repo-name/index.html?api=true&q=lesson

The API responses will be in JSON format that your Android app can easily parse. This approach works with GitHub Pages since it's still serving static files, but provides the API-like functionality your Android app needs.