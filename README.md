# Frontend Development Test

## Project Overview
This is a frontend application built with Next.js that fetches and displays research paper data from the provided API. The primary goal of this project is to demonstrate best practices in data fetching, UI design, and interactivity. The application focuses on speed, quality, optimization, and clean coding.

Users can search, filter, sort, and paginate through research papers. Each paper is displayed in a card UI, which contains relevant information such as title, authors, journal name, DOI, impact factor, and links to PDFs or media (if available). A detailed view is available on request, allowing users to access more comprehensive paper metadata.
## Getting Started

To run the development server locally, follow these steps:

1. Clone the repository:
   ```bash
  git clone https://github.com/janardhankhandagle/frontend-research-paper-app.git
  cd frontend-research-paper-app


```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Folder Structure
components/: Contains UI components such as SearchBar, PaperCard, PaperModal, and Pagination.
styles/: SCSS files for styling components using SCSS modules. Each component has a corresponding .module.scss file.
utils/: Contains utility functions like api.js for handling API requests.
Data Fetching
All data is fetched asynchronously from the EasyDash API (https://easydash.enago.com/acceptedpapers). API calls are managed in a utility file (api.js), ensuring modularity and reusability. The app handles loading, success, and error states clearly to provide a smooth user experience.

UI Display - Card Components
Title
Authors
Year
Journal Name
Impact Factor
PDF/Media Links (if available)
The card layout is clean and professional, with placeholders for images when necessary. This ensures that the design is consistent and user-friendly.

Search Functionality
A search bar is provided to filter papers by keywords. Users can select a category to search in, such as:
Title
Author
Journal
The search results are updated dynamically as the user types or selects a category. This feature provides an intuitive way to find relevant papers quickly.

Sorting
Title (ascending/descending)
Year (ascending/descending)
Impact Factor (ascending/descending)
Sorting controls are implemented to allow users to easily organize papers in the way that best suits their needs.
Pagination
Client-side pagination is used to break up large datasets into smaller, manageable chunks. Pagination controls allow users to navigate between pages with a clear indication of the current page and total results.

Details View
Each paper card includes a "View Details" button. Clicking on this button opens a detailed view of the paper in a modal or on a new page. The detailed view includes complete metadata such as:
Title
Authors
Journal

SCSS & Styling
SearchBar.module.scss: Styles for the search bar component, including the input field and category dropdown.
PaperCard.module.scss: Styles for the paper card, including layout for paper details, author names, journal titles, and impact factor.
PaperDetails.module.scss: Modal styles for displaying full paper details.
pagination.module.scss: Pagination controls for navigating between pages.
SCSS variables are defined for colors, font sizes, and spacing to maintain consistency across the app.
