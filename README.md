```markdown
# Static Sales Report Calculator

## Summary

This project is a single-page static website designed to calculate and display sales information from an included `data.csv` file. It processes the data client-side using JavaScript and presents both the total sales figure and a detailed breakdown of individual product sales in a Bootstrap table. The "Sales Report" page is styled with Bootstrap 5 for a clean and responsive interface. The total sales sum is displayed within an HTML element with the ID `total-sales`, and the product sales table is rendered below it.

## Setup

This is a static website, meaning there is no server-side setup or local installation required. All calculations are performed directly in the web browser.

## Usage

To view the Sales Report:

1.  **Open the `index.html` file:** Navigate to the project directory and open the `index.html` file directly in your preferred web browser.
2.  **View Deployed Page:** If the project is hosted on a web server (e.g., GitHub Pages), simply navigate to its live deployed URL.

Upon loading, the page will automatically fetch `data.csv`, process the data to calculate the total sales, and display both the overall sum and a table detailing individual product sales in their respective areas.

## Code Explanation

This project combines HTML, CSS (Bootstrap 5), and JavaScript to achieve its goal:

*   **`index.html`**:
    This file provides the structure of the single-page application. It includes the necessary Bootstrap 5 CSS for styling, sets the page title to "Sales Report", and contains:
    *   An HTML element (e.g., a `<span>` or `<div>`) with the ID `total-sales` where the calculated total sum will be displayed.
    *   A designated area (e.g., a `<div>`) where the Bootstrap table detailing individual product sales will be rendered dynamically by JavaScript.
*   **`data.csv`**:
    This comma-separated values file contains the raw sales data that the application processes. It is expected to be accessible by the client-side JavaScript.
*   **JavaScript (e.g., `script.js` or inline within `index.html`)**:
    The core logic is implemented in JavaScript. It is responsible for:
    *   Fetching the `data.csv` file from the same directory or a specified path.
    *   Parsing the CSV content to extract individual product sales figures (e.g., Apple, Banana, Orange with their respective amounts).
    *   Calculating the sum of all sales.
    *   Generating the HTML for a Bootstrap table (using `class="table"`) with "Product" and "Sales" as headers, populated with each product and its corresponding sales amount.
    *   Updating the HTML element with `id="total-sales"` to display the final calculated sum on the page.
    *   Injecting the generated product sales table into the designated area on the page, typically below the total sales figure.
*   **Bootstrap 5**:
    Used for basic styling and responsiveness, including the `table` class for the product sales breakdown, ensuring a clean and modern user interface without custom CSS.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute the code for personal or commercial use. See the [LICENSE](LICENSE) file (if present) for more details.
```