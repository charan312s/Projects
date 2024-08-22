<!DOCTYPE html>
<html lang="en">
<head>

</head>
<body>
    <h1>Flipkart Data Extraction Cleaning</h1>
    <p>This project involves cleaning and processing the data extracted from Flipkart's mobile search results. The data cleaning process focuses on improving the usability and quality of the extracted data for further analysis.</p>

<h2>Project Structure</h2>
<ul>
    <li><code>Flipkart Extracted Data Cleaning.ipynb</code>: The main Jupyter Notebook containing the code for data cleaning and processing.</li>
    <li><code>processed_cleaned_data.csv</code>: The output CSV file with cleaned and processed data.</li>
</ul>

<h2>Data Cleaning Steps</h2>
<ol>
    <li><strong>Battery Column Processing:</strong> Extracted integer values from the battery information to provide a uniform format.</li>
    <li><strong>Warranty Column Processing:</strong> Converted warranty durations from months to years and removed unnecessary terms.</li>
    <li><strong>And many more</li>
</ol>

<h2>Requirements</h2>
<p>To run the data cleaning code, you'll need the following Python libraries:</p>
<ul>
    <li><code>pandas</code></li>
    <li><code>regular expression</code></li>
</ul>
<p>You can install these dependencies using the following command:</p>
<pre><code>pip install pandas</code></pre>
<pre><code>pip install re</code></pre>

<h2>DataFrame Structure</h2>
<p>After cleaning, the data is stored in a Pandas DataFrame with the following attributes:</p>
<ul>
    <li><strong>actual_price</strong>: The actual price of the mobile product.</li>
    <li><strong>selling_price</strong>: The selling price of the mobile product after discounts.</li>
    <li><strong>offer</strong>: Discount offer information.</li>
    <li><strong>rating(outof5)</strong>: Customer rating out of 5.</li>
    <li><strong>no_of_ratings</strong>: Number of ratings received.</li>
    <li><strong>no_of_reviews</strong>: Number of reviews received.</li>
    <li><strong>battery</strong>: Battery capacity (in mAh).</li>
    <li><strong>processor</strong>: Processor details.</li>
    <li><strong>warranty</strong>: Warranty duration in years.</li>
    <li><strong>product_link</strong>: Link to the product page on Flipkart.</li>
    <li><strong>model_name</strong>: Model name of the mobile product.</li>
    <li><strong>extracted_memory</strong>: Memory size extracted from the product information.</li>
    <li><strong>RAM</strong>: RAM size of the mobile product.</li>
    <li><strong>ROM</strong>: ROM size of the mobile product.</li>
    <li><strong>expandable_memory</strong>: Information on expandable memory.</li>
    <li><strong>screen_size</strong>: Screen size of the mobile product.</li>
    <li><strong>display_type</strong>: Display type (e.g., Retina, Normal Display).</li>
    <li><strong>rear_camera</strong>: Rear camera specifications.</li>
    <li><strong>front_camera</strong>: Front camera specifications.</li>
</ul>

<h2>Example DataFrame</h2>
<table border="1">
    <thead>
        <tr>
            <th>actual_price</th>
            <th>selling_price</th>
            <th>offer</th>
            <th>rating(outof5)</th>
            <th>no_of_ratings</th>
            <th>no_of_reviews</th>
            <th>battery</th>
            <th>processor</th>
            <th>warranty</th>
            <th>product_link</th>
            <th>model_name</th>
            <th>extracted_memory</th>
            <th>RAM</th>
            <th>ROM</th>
            <th>expandable_memory</th>
            <th>screen_size</th>
            <th>display_type</th>
            <th>rear_camera</th>
            <th>front_camera</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>69900.0</td>
            <td>58999.0</td>
            <td>15% off</td>
            <td>4.6</td>
            <td>255.0</td>
            <td>9906.0</td>
            <td>Unknown</td>
            <td>A15 Bionic Chip, 6 Core Processor</td>
            <td>1 Year</td>
            <td><a href="https://www.flipkart.com/apple-iphone-14-starlight-128-gb/p/itm2b717b2e91b67">Link</a></td>
            <td>APPLE iPhone 14</td>
            <td>128 GB</td>
            <td>Unknown</td>
            <td>128 GB</td>
            <td>Not Expandable</td>
            <td>15.49 cm</td>
            <td>Retina</td>
            <td>24.0MP</td>
            <td>12MP</td>
        </tr>
    </tbody>
</table>

<h2>Important Notes</h2>
<p>Ensure that the data cleaning steps are consistent with the current structure of the dataset. Adjust the cleaning logic as needed if the dataset structure changes.</p>

<h2>Troubleshooting</h2>
<ul>
    <li><strong>Data Issues:</strong> Verify that the data follows the expected format before applying transformations. Check for any inconsistencies or missing values.</li>
</ul>

<h2>Contributing</h2>
<p>Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.</p>
</body>
</html>
