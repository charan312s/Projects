<!DOCTYPE html>
<html lang="en">
<head>

</head>
<body>
    <h1>Flipkart Data Web Scraping</h1>
    <p>This project, developed in December 2023, involves web scraping data from Flipkart's mobile search results using Python. The extracted data can be used for various analyses, such as price comparisons, product reviews, and feature comparisons.</p>

<h2>Project Structure</h2>
<ul>
    <li><strong>Flipkart Data Web Scraping.ipynb</strong>: The main Jupyter Notebook containing the code for web scraping Flipkart's mobile search results.</li>
</ul>

<h2>Requirements</h2>
<p>To run the code in this project, you'll need the following Python libraries:</p>
<ul>
    <li><code>requests</code></li>
    <li><code>beautifulsoup4</code></li>
    <li><code>pandas</code></li>
</ul>
<p>You can install these dependencies using the following command:</p>
<pre><code>pip install requests beautifulsoup4 pandas</code></pre>

<h2>DataFrame Structure</h2>
<p>The extracted data is stored in a Pandas DataFrame, with the following attributes:</p>
<ul>
    <li><strong>Product Name</strong>: The name of the mobile product listed on Flipkart.</li>
    <li><strong>Price</strong>: The price of the mobile product as listed on the website.</li>
    <li><strong>Rating</strong>: The customer rating for the product, typically out of 5.</li>
    <li><strong>Number of Reviews</strong>: The number of reviews the product has received.</li>
    <li><strong>Features</strong>: Key features of the mobile product, which may include specifications such as RAM, storage capacity, camera details, etc.</li>
    <li><strong>Availability</strong>: Indicates whether the product is in stock or not.</li>
</ul>

<h3>Example DataFrame:</h3>
<table border="1">
    <thead>
        <tr>
            <th>Product Name</th>
            <th>Price</th>
            <th>Rating</th>
            <th>Number of Reviews</th>
            <th>Features</th>
            <th>Availability</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Samsung Galaxy M32</td>
            <td>₹14,999</td>
            <td>4.2</td>
            <td>34,500</td>
            <td>6GB RAM, 128GB Storage, 64MP Camera</td>
            <td>In Stock</td>
        </tr>
        <tr>
            <td>Redmi Note 10 Pro</td>
            <td>₹16,999</td>
            <td>4.5</td>
            <td>40,000</td>
            <td>8GB RAM, 128GB Storage, 108MP Camera</td>
            <td>In Stock</td>
        </tr>
        <tr>
            <td>Realme 8 Pro</td>
            <td>₹17,499</td>
            <td>4.3</td>
            <td>28,000</td>
            <td>6GB RAM, 128GB Storage, 48MP Camera</td>
            <td>Out of Stock</td>
        </tr>
    </tbody>
</table>

<h2>Important Note</h2>
<p>This project was originally developed in December 2023. Since then, the Flipkart website has undergone some changes, including modifications to class names and other structural elements. These changes may cause the current code to break or not function as intended.</p>
<h3>Steps to Update the Code:</h3>
<ol>
    <li>Review the Flipkart webpage structure by inspecting the updated HTML elements.</li>
    <li>Modify the selectors in the BeautifulSoup parsing logic to match the new class names and structure.</li>
</ol>

<h2>Troubleshooting</h2>
<h3>500 Internal Server Error:</h3>
<p>This error may occur if the server is unable to process the request. You can try changing the User-Agent in the headers or running the code at a later time.</p>

<h3>Rate Limiting:</h3>
<p>If you encounter rate limiting, consider slowing down your requests or using a proxy to avoid getting blocked.</p>

<h2>License</h2>
<p>This project is licensed under the MIT License. See the LICENSE file for details.</p>

<h2>Contributing</h2>
<p>Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.</p>
</body>
</html>
