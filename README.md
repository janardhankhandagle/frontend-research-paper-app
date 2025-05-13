# Frontend Development Test

## Project Overview

This is a frontend application built with **Next.js** that fetches and displays research paper data from the provided API. The goal of this project is to demonstrate best practices in **data fetching**, **UI design**, and **interactivity**. The app focuses on **speed**, **quality**, **optimization**, and **clean coding**.

The application allows users to search, filter, sort, and paginate research papers. It also includes a card UI design to display key information for each paper, with a detailed view available on request.

## Getting Started

To run the development server locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <project-directory>

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

This project was bootstrapped with Next.js 14.0.0 and includes SCSS modules for styling. Here's a brief overview of the key directories and files:

components/: Contains the UI components like SearchBar, PaperCard, PaperModal, and Pagination.

styles/: SCSS files to style components using SCSS modules. Each component has its own corresponding .module.scss file.

utils/: Contains utility functions like api.js for handling API requests.
 Data Fetching
All data is fetched asynchronously from the EasyDash API (https://easydash.enago.com/acceptedpapers).

API calls are managed in a utility file (api.js), ensuring modularity and reusability.

The app handles loading, success, and error states clearly.

2. UI Display - Card Components
Each paper is displayed as a Card UI with the following details:

Title

Authors

Year

Journal Name

DOI

Impact Factor

PDF/Media Links (if available)

The card layout is clean and professional, with placeholders for images where necessary.

3. Search Functionality
A search bar is provided to filter papers by keywords.

Users can select a category to search in, such as:

Title

Author

Journal

The search results update dynamically as the user types or selects a category.

4. Sorting
Papers can be sorted by:

Title (ascending/descending)

Year (ascending/descending)

Impact Factor (ascending/descending)

5. Pagination
Implemented client-side pagination to break up large data sets into smaller, manageable chunks.

The pagination control allows users to navigate between pages, with a clear indication of the current page and total results.

6. Details View
Each paper card includes a View Details button.

Clicking on the button opens a detailed view of the paper in a modal or a new page.

The detailed view shows complete metadata such as:

Title

Authors

Journal

Abstract (if available)

DOI

Impact Factor

7. Customization & Optimization
The card components are designed with customization in mind. Elements such as the position of media and text can be rearranged as needed.

SCSS variables are used for consistent theming and color management across the app.

The application is built with performance in mind, particularly for handling large datasets.

8. Bonus (Optional)
Skeleton loaders are displayed during data fetch to enhance the user experience.

Debounce is applied to the search input to prevent unnecessary API calls.

A download button is provided for PDF links when available.

SCSS & Styling
The application uses SCSS modules for styling to ensure that styles are scoped to individual components. Here's a breakdown of the SCSS structure:

SearchBar.module.scss: Styles for the search bar component, including the input field and category dropdown.

PaperCard.module.scss: Styles for the paper card, including layout for paper details, author name, journal title, and impact factor.

PaperDetails.module.scss: Modal styles for displaying full paper details.

pagination.module.scss: Pagination controls for navigating between pages.

SCSS variables are defined for colors, font sizes, and spacing to maintain consistency across the app.