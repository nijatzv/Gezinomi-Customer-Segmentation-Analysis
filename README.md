<h1>Gezinomi Customer Segmentation Analysis</h1>

<h2>Project Overview</h2>
<p>
This project involves creating level-based sales definitions for Gezinomi, a travel company, to segment customers based on sales data and customer characteristics. By implementing a rule-based classification model, the project aims to predict potential revenue from new customers according to these defined segments. For instance, we may estimate how much a customer who plans to visit an all-inclusive hotel in Antalya during peak season could generate in revenue. This segmentation analysis enables more effective marketing, personalized customer engagement, and optimized sales strategies for Gezinomi.
</p>

<h2>Business Problem</h2>
<p>
Gezinomi seeks to enhance its revenue estimation model by segmenting customers into meaningful groups. These segments allow the company to:
</p>
<ul>
    <li>Target high-value customer segments, enhancing marketing efficiency.</li>
    <li>Forecast revenue from different customer types.</li>
    <li>Personalize offerings based on customer preferences, boosting engagement and satisfaction.</li>
</ul>

<h2>Data Set</h2>
<p>
The dataset, <code>gezinomi_miuul.xlsx</code>, records each transaction in detail, capturing all sales information for a given booking. Since the dataset includes multiple purchases per customer, it allows for a comprehensive view of recurring behaviors and spending patterns.
</p>

<h3>Key Variables</h3>
<ul>
    <li><b>SaleID</b>: Unique identifier for each sale.</li>
    <li><b>SaleDate</b>: Date the sale was made.</li>
    <li><b>CheckInDate</b>: Date the customer checked in.</li>
    <li><b>Price</b>: Amount spent for each booking.</li>
    <li><b>ConceptName</b>: Type of booking package (e.g., All-Inclusive, Half-Board).</li>
    <li><b>SaleCityName</b>: City of the hotel.</li>
    <li><b>CInDay</b>: Day of the week for check-in.</li>
    <li><b>SaleCheckInDayDiff</b>: Days between sale and check-in date.</li>
    <li><b>Season</b>: Season during the booking (e.g., High, Low).</li>
</ul>

<h3>Additional Attributes</h3>
<p>
Further details in the dataset, such as weekday vs. weekend check-ins and seasonal demand, enhance the model’s precision by contextualizing spending patterns.
</p>

<h2>Project Tasks</h2>
<ol>
    <li><b>Data Cleaning and Preprocessing</b>
        <ul>
            <li>Prepare the dataset by handling missing values, formatting fields, and creating derived variables.</li>
        </ul>
    </li>
    <li><b>Feature Engineering</b>
        <ul>
            <li>Develop additional features, such as booking lead time categories, to capture customer intent.</li>
            <li>Convert <code>SaleCheckInDayDiff</code> into categorical segments like "Last Minuters," "Potential Planners," "Planners," and "Early Bookers."</li>
        </ul>
    </li>
    <li><b>Rule-Based Classification and Segmentation</b>
        <ul>
            <li>Using attributes such as city, booking concept, season, and booking timing, define level-based segments for customer classification.</li>
            <li>Create the <code>sales_level_based</code> variable, combining city, package type, and season, to represent specific customer segments.</li>
        </ul>
    </li>
    <li><b>Segment Analysis</b>
        <ul>
            <li>Divide the newly defined segments into four categories based on average spending potential.</li>
            <li>For each segment, calculate key metrics like mean, max, and sum of revenue, enabling comparative analysis across segments.</li>
        </ul>
    </li>
    <li><b>Revenue Prediction for New Customers</b>
        <ul>
            <li>Using the defined segments, predict the revenue potential for new customer profiles, such as those traveling during peak seasons to specific destinations.</li>
        </ul>
    </li>
</ol>

<h2>Conclusion</h2>
<p>
Through this segmentation analysis, Gezinomi gains actionable insights into customer behavior and revenue potential, supporting data-driven decisions to maximize profitability and customer satisfaction. The segmentation model not only informs marketing and sales strategies but also positions Gezinomi for personalized service offerings, improving its competitive advantage in the travel industry.
</p>
