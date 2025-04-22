# Spotify_Data_Analysis_SQL

![image](https://github.com/user-attachments/assets/4bf33359-ddd0-4723-89e0-8af9fcdb4879)

## 📑 Contents

- [**🌐 Introduction**](#-introduction)
- [**💾 Data Setup in SQL Workbench**](#-data-setup-in-sql-workbench)
- [**🔍 Exploring the Dataset**](#-exploring-the-dataset)
- [**🔍 Analytical Insights**](#-analytical-insights)
- [**⚙️ SQL Techniques**](#️-sql-techniques)
- [**💡 Key Findings**](#-key-findings)
- [**📂 Data Source**](#-data-source)
- [**🛠️ Skills Demonstrated**](#️-skills-demonstrated)
- [**🚀 Future Scope**](#-future-scope)
  
The Spotify Data Analysis Project: In today's changing world, data analysis has become crucial in fields such as business, research, and meteorology. This project showcases the role that data plays in making decisions, advancing research initiatives, and even predicting weather patterns.

The immense potential of data analysis is evident in this project, which focuses on extracting insights from music-related datasets using SQL queries and aggregate functions (Sum, Order by, Group by, Rank, Limit,  etc.). At its core, Spotify takes center stage as an audio streaming giant with captivating features like seamless song sharing and synchronized lyrics display.

Throughout this project, I delved into the realm of data using SQL’s built-in functions and JOIN operations. From analyzing to visualizing the data , this project covers all aspects of data processing. The interactive environment provided by SQL editor as MySQL Workbench enhanced my experience by allowing me to engage with the data and discover patterns.

Through the Spotify Data Analysis Project, I not only sharpened my SQL querying skills but also gained a deep understanding of how data intertwines with the world of music. This journey provided insights and equipped me with confidence to undertake similar projects in the future.

Don't forget to follow and star ⭐ the repository if you find it valuable.

Tools Used🛠️:My Sql Workbench

Data Set📂:[Spotify Dataset](https://drive.google.com/drive/folders/1bB1oyYPT9Nde5LxD_HCSWphku5BLvfHG?usp=sharing)

## 💾 Data Setup in SQL Workbench

In this project, I worked with a music database using MySQL Workbench. The database includes several interrelated tables that reflect real-world entities in a music store environment.

- album: Contains details about each album, including Album ID and Title.

- artist: Holds information about artists, including their unique Artist ID and Name.

- customer: Stores customer data such as names, addresses, and contact details.

- employee: Represents employees of the store with their roles and reporting structure.

- genre: Lists various music genres with their Genre IDs.

- invoice: Captures billing information including Invoice ID, Customer ID, Date, and Total.

- invoice_line: Stores line-by-line details of each invoice, such as Track ID, Quantity, and Unit Price.

- media_type: Contains types of media formats like MPEG audio, AAC audio, etc.

- playlist: Stores playlist names and their IDs.

- playlist_track: Maps tracks to their respective playlists.

- track: Contains metadata for each song, including Name, Album ID, Media Type, Genre, Composer, Duration, and Price.

These tables were queried using SQL to perform various data analysis operations such as aggregation, joins, filtering, sorting, and ranking to extract business insights from the music data.

## 🔍 Exploring the Dataset

After setting up the database in MySQL Workbench, the initial step was to explore and understand the structure of each table. Using SQL queries like SELECT * FROM table_name LIMIT 5;, I previewed the contents of key tables to get a sense of the data available for analysis.

This exploratory phase involved:

- Reviewing column names, data types, and sample values

- Identifying primary and foreign key relationships between tables

- Understanding the volume and variety of data in each table

- Checking for any missing or duplicate values

- Mapping out how tables such as track, artist, genre, invoice, and customer are interconnected for future joins

This step helped me plan relevant queries and design a structured approach to uncover meaningful insights from the dataset.


```sql

# Viewing the Data
select * from album;
select * from artist;
select * from customer;
select * from employee;
select * from genre;
select * from invoice;
select * from invoice_line;
select * from media_type;
select * from playlist;
select * from playlist_track;
select * from track;
```

```sql
# Viewing the Data
select * from album;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![album](https://github.com/user-attachments/assets/0dd4846a-09a2-4a4d-8f4b-d8cedf48ebed)

```sql
# Viewing the Data
select * from artist;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![Artist](https://github.com/user-attachments/assets/ca5a02d9-b742-4b3d-af41-a0b94a6c79b4)

```sql
# Viewing the Data
select * from customer;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![customer](https://github.com/user-attachments/assets/4bd8c09c-efcb-4a22-a1eb-23a83bbadae1)


```sql
# Viewing the Data
select * from employee;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![employee](https://github.com/user-attachments/assets/7f717053-a53f-4b42-8ea4-18e722c1a236)


```sql
# Viewing the Data
select * from genre;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![genre](https://github.com/user-attachments/assets/50a97241-9cf2-4e8e-9d41-f03058613a6c)


```sql
# Viewing the Data
select * from invoice;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![invoice](https://github.com/user-attachments/assets/4e2ee481-a340-4322-84f9-2f71da55f924)


```sql
# Viewing the Data
select * from invoice_line;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![invoice_line](https://github.com/user-attachments/assets/93da5a2d-70bc-42bc-8af6-ebdfdf4000f2)


```sql
# Viewing the Data
select * from media_type;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![media_type](https://github.com/user-attachments/assets/de2a4437-c58f-41b7-8fc1-090dcf2e1d5f)


```sql
# Viewing the Data
select * from playlist;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![playlist](https://github.com/user-attachments/assets/45a52cce-8766-407e-aec4-622f65019ef7)


```sql
# Viewing the Data
select * from playlist_track;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![playlist_track](https://github.com/user-attachments/assets/5171936b-3888-4a75-969f-6d9ae3bb64fa)


```sql
# Viewing the Data
select * from track;
```

**Note:** The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![track](https://github.com/user-attachments/assets/e3b84873-f398-434a-af4e-21a7a85bc746)

## 🔍 Analytical Insights

- ### **`Senior Employee Identification`**

Identified the senior-most employee based on job title hierarchy to assign project leadership.

```sql
# Viewing the Data
select title, first_name,last_name,levels from employee
order by levels desc
limit 1;

```
![Senior Employee Identification](https://github.com/user-attachments/assets/af403c4d-e9a4-4920-8b21-5db2f97a9ff7)

Query Explanation:

This query identifies the organization's most senior employee by checking their hierarchical level. It selects the employee's job title, full name, and seniority level from the database. The results are sorted in descending order to display the highest-ranking employee first. By limiting output to just one record, we pinpoint the single most qualified leader. This data-driven approach ensures objective leadership selection based on established company structure.

- ### **`Invoice Volume by Country`**

Determined the country generating the highest number of invoices for targeted marketing.

```sql
# Viewing the Data
select * from invoice;
select billing_country,count(*) as no_of_invoice
 from invoice
group by billing_country
order by no_of_invoice desc
limit 1;

```
![Invoice Volume by Country](https://github.com/user-attachments/assets/afccaf4d-0880-424c-b4d0-446c611af659)

Query Explanation:

This analysis identifies which country generates the highest volume of invoices. The query first examines all invoice records, then groups them by billing country to count transactions per nation. By sorting the results in descending order and limiting to the top result, we pinpoint the single country with the most invoices. This reveals the organization's strongest geographic market for sales activity.

-  ### **`Top 3 Invoice Values`**

Calculated the monetary value of the top 3 highest invoices to understand premium transactions.

```sql
# Viewing the Data
select * from invoice
order by total desc
limit 3;

```
![Top three values](https://github.com/user-attachments/assets/832592f6-89a0-464b-b45e-e4c0b2e5e77f)

Query Explanation:

This SQL query selects all columns from the invoice table, then sorts the results in descending order by the total column to show the highest invoice amounts first. By adding LIMIT 3, it returns only the top three invoices with the largest totals. The output displays complete invoice details, including ID, customer information, billing address, and the sorted total amount. From the results, we can see that invoice #183 (€23.76) is the highest, followed by two invoices (#92 and #526) tied at $19.80 each—one from Canada and another from the Czech Republic. This type of query is useful for financial analysis, helping businesses quickly identify their most valuable transactions.

-  ### **`Promotional Festival Location`**

Analyzed revenue by city to select the optimal location for a music festival based on customer spending.

```sql
# Viewing the Data
select billing_city,sum(total) as Totals from invoice
group by billing_city
order by sum(total) desc
limit 1;
```
![Promotional Festival Location](https://github.com/user-attachments/assets/52158c5f-fd96-4710-bbc8-3dff33213cdf)

Query Explanation:

This SQL query analyzes invoice data to identify which city generated the highest total revenue. It works in three key steps: First, it groups all invoices by their billing_city using the GROUP BY clause. Then it calculates the sum of the total column for each city, labeling this aggregated value as "Totals". The ORDER BY sum(total) DESC sorts these city totals in descending order, putting the highest-revenue city at the top. Finally, the LIMIT 1 restriction returns only this top-performing city. The result shows Prague as the highest-grossing location with total revenues of approximately 273.24 currency units, making it the most successful city for this promotional festival based on invoice totals. This type of analysis helps businesses understand their best-performing markets for strategic decision-making.


-  ### **`Best Customer Recognition`**
  
Evaluated total customer expenditure to declare the highest-spending customer as "Best Customer".

```sql
# Viewing the Data
select c.first_name,c.last_name,sum(total) as Total from customer as c
inner join invoice as i on c.customer_id = i.customer_id
group by c.first_name,c.last_name
order by Total desc
limit 1;
```

![Best Customer Recognition](https://github.com/user-attachments/assets/9b36a213-b4ad-4434-8962-e2c527205bf6)

Query Explanation:

This SQL query identifies the top-spending customer by analyzing purchase history across joined customer and invoice data. First, it connects the customer and invoice tables through an inner join using matching customer_id values. The query then groups the combined records by each customer's first and last name while calculating their cumulative spending using sum(total) as Total. By sorting these aggregated totals in descending order with ORDER BY Total DESC and limiting to just one result with LIMIT 1, the query efficiently pinpoints the highest-value customer. The output reveals František Wichtelovič as the best customer with total purchases worth approximately 144.54 currency units, making them the clear candidate for special recognition or loyalty rewards. This analysis provides valuable insight for customer relationship management and targeted marketing strategies.

-  ### **`Rock Music Audience Profile`**

Extracted customer details exclusively listening to Rock music for targeted engagement.

```sql
# Viewing the Data
select distinct c.first_name,c.last_name,c.email,g.name as Gerne  from customer as c
inner join invoice as i on c.customer_id = i.customer_id
inner join invoice_line as il on i.invoice_id = il.invoice_id
inner join track as t on t.track_id = il.track_id
inner join genre as g  on t.genre_id = g.genre_id
where g.name = "Rock"
order by c.email
```

Note: The image displays only a partial view of the complete results due to screenshot limitations. For the full dataset and comprehensive tables, please execute these queries directly in your SQL environment or refer to the complete result exports available in this repository's data outputs folder.

![Rock Music Audience Profile](https://github.com/user-attachments/assets/4a6b94e4-5e53-4ffa-be4d-d5156455628f)

Query Explanation:

This SQL query builds a detailed profile of rock music listeners by analyzing customer purchase data across multiple connected database tables. The query starts with the customer table and progressively joins four additional tables: invoice, invoice_line, track, and genre - creating a complete chain from customer identity to musical preferences. By setting the condition WHERE g.name = "Rock", it filters to only include customers who purchased tracks classified under the rock genre. The SELECT DISTINCT clause ensures each customer appears only once in the results, even if they made multiple rock purchases. Finally, the results are organized alphabetically by email address (ORDER BY c.email) for easy reference. The output reveals a diverse international audience of rock music fans, with customers from countries including Canada, Brazil, Austria, Norway, France, Belgium, Argentina, Spain, and others - demonstrating the global appeal of rock music across this customer base. This type of audience analysis helps music businesses understand their core demographics and tailor marketing campaigns accordingly.


-  ### **`Top 10 Rock Music Artists`**

Identified artists with the highest Rock music contributions for festival invitations.

```sql
# Viewing the Data
SELECT ar.artist_id,ar.name,COUNT(t.track_id) AS number_of_songs FROM track t
JOIN album al ON al.album_id = t.album_id
JOIN artist ar ON ar.artist_id = al.artist_id
JOIN genre g ON g.genre_id = t.genre_id
where g.name ="Rock"
GROUP BY ar.artist_id, ar.name
ORDER BY number_of_songs DESC
LIMIT 10;

```

![Top 10 Rock Music Artists](https://github.com/user-attachments/assets/7b115211-31c4-473d-8cc3-16aae87a5ba9)

Query Explanation:

This SQL query identifies the top 10 rock artists based on their number of available tracks in the database. The analysis begins by connecting five key tables: track, album, artist, and genre through a series of JOIN operations that link tracks to their respective albums and artists while filtering for only rock genre tracks (WHERE g.name = "Rock"). By grouping the results by artist ID and name (GROUP BY ar.artist_id, ar.name), then counting the tracks per artist (COUNT(t.track_id) AS number_of_songs), the query quantifies each rock artist's representation in the catalog. The results are then sorted in descending order by track count (ORDER BY number_of_songs DESC) and limited to the top 10 performers (LIMIT 10). The output reveals AC/DC as the dominant rock artist with 18 tracks, followed by Aerosmith (15 tracks), and Audioslave and Led Zeppelin tied with 14 tracks each - providing valuable insights into the most prolific rock artists in this music collection, which could inform inventory decisions, promotional campaigns, or customer recommendations.


-  ### **`Genre Popularity by Country`** 

Mapped the most popular music genre per country to inform inventory and marketing strategies.

```sql
# Viewing the Data
WITH popular_genre AS (
SELECT COUNT(il.quantity) AS purchases,c.country,g.name AS genre_name,g.genre_id,  
ROW_NUMBER() OVER(PARTITION BY c.country ORDER BY COUNT(il.quantity) DESC) AS RowNo
FROM invoice_line il
JOIN invoice i ON i.invoice_id = il.invoice_id 
JOIN customer c ON c.customer_id = i.customer_id 
JOIN track t ON t.track_id = il.track_id 
JOIN genre g ON g.genre_id = t.genre_id 
GROUP BY c.country, g.name, g.genre_id
    ORDER BY c.country ASC, purchases DESC
)
SELECT * 
FROM popular_genre 
WHERE RowNo <= 1;

```

![Genre Popularity by Country](https://github.com/user-attachments/assets/13d081a8-fbe7-409c-a1f0-1b2cd75c93f6)

Query Explanation:

This SQL query analyzes music genre popularity across different countries to reveal global listening trends. By connecting purchase records with customer locations and track genres, it identifies each country's most-bought music style. The results show rock music dominates overwhelmingly, being the top genre in 21 of the 24 countries analyzed - including major markets like the USA (70 purchases), Canada (57), United Kingdom (47), and Brazil (26). Only Norway and Spain break this pattern, preferring metal instead. The analysis uses a sophisticated ranking system that first counts all genre purchases per country, then uses ROW_NUMBER() to identify each nation's clear favorite. This reveals rock's universal appeal while highlighting rare regional variations, providing valuable insights for music platforms to customize their offerings - like emphasizing rock playlists globally while potentially adding more metal content for Scandinavian and Spanish audiences. The query's efficient structure processes complex data relationships to deliver these market insights in a clear, country-by-country breakdown.



-  ### **`Top Customers by Country`** 

Pinpointed the highest-spending customer per country for loyalty rewards.

```sql
# Viewing the Data
WITH Customer_with_country AS (
    SELECT 
        c.customer_id,
        c.first_name,
        c.last_name,
        i.billing_country,
        SUM(i.total) AS total_spending,
        ROW_NUMBER() OVER(PARTITION BY i.billing_country ORDER BY SUM(i.total) DESC) AS RowNo 
    FROM invoice i
    JOIN customer c ON c.customer_id = i.customer_id
    GROUP BY 
        c.customer_id,
        c.first_name,
        c.last_name,
        i.billing_country
    ORDER BY 
        i.billing_country ASC,
        total_spending DESC
)
SELECT * FROM Customer_with_country 
WHERE RowNo <= 1
ORDER BY total_spending DESC;
```

![Top Customers by Country](https://github.com/user-attachments/assets/f64eea01-df60-43e9-9d53-0e5ee1729f83)

Query Explanation:

This SQL query identifies the highest-spending customer in each country by analyzing purchase data. First, it connects customer information with their invoice records to calculate each customer's total spending. The query then organizes customers by country and ranks them based on purchase amounts, assigning the top spender in each country a rank of 1. After establishing these rankings, the query filters to show only the top-ranked customer from each nation. Finally, it presents these leading customers sorted by total spending in descending order.

The results reveal the Czech Republic's customer as the leading global spender with 144.54 inpurchases,followed by Ireland′stop customer at 144.54 inpurchases. The dataset covers 24 countries, with spending values ranging from 144.54 down to  37.62 in Denmark. This analysis provides valuable insights into international purchasing behaviors and regional market strengths.



## ⚙️ SQL Techniques

This project demonstrates a variety of SQL techniques applied to real-world business problems:

- Data Filtering
Used WHERE clauses to extract specific records based on conditions.

- Sorting Results
Applied ORDER BY to arrange data in ascending or descending order.

- Aggregate Functions
Used SUM(), COUNT(), AVG() to calculate total sales, number of customers, average invoices, etc.

- Grouping Data
Used GROUP BY to summarize data by country, customer, genre, and more.

- Joining Multiple Tables
Connected multiple related tables using INNER JOIN to retrieve complete information.

- Common Table Expressions (CTEs)
Simplified complex queries using WITH clauses to break them into readable parts.

- Window Functions
Applied ROW_NUMBER() to rank customers and identify top spenders per region or genre.

- Subqueries
Used nested queries to solve step-by-step problems like finding top-selling genres.

- Aliasing
Used AS to rename columns and tables for better readability.

- LIMIT and DISTINCT
Limited output results and removed duplicates where necessary.





## 📂 Data Source

Data Set📂:
[Spotify Dataset](https://drive.google.com/drive/folders/1bB1oyYPT9Nde5LxD_HCSWphku5BLvfHG?usp=sharing)

- album: Contains details about each album, including Album ID and Title.

- artist: Holds information about artists, including their unique Artist ID and Name.

- customer: Stores customer data such as names, addresses, and contact details.

- employee: Represents employees of the store with their roles and reporting structure.

- genre: Lists various music genres with their Genre IDs.

- invoice: Captures billing information including Invoice ID, Customer ID, Date, and Total.

- invoice_line: Stores line-by-line details of each invoice, such as Track ID, Quantity, and Unit Price.

- media_type: Contains types of media formats like MPEG audio, AAC audio, etc.

- playlist: Stores playlist names and their IDs.

- playlist_track: Maps tracks to their respective playlists.

- track: Contains metadata for each song, including Name, Album ID, Media Type, Genre, Composer, Duration, and Price.



## 🛠️ Skills Demonstrated

- SELECT Statements
Basic data retrieval from multiple tables using SELECT *, SELECT column_name, etc.

- Filtering with WHERE Clause
Used to filter records based on specific conditions, e.g., WHERE g.name = "Rock".

- Sorting with ORDER BY
Sorted data in ascending/descending order using ORDER BY, e.g., ORDER BY total DESC.

- Aggregation Functions
Used functions like SUM(), COUNT() to calculate totals and counts.

- GROUP BY Clause
Grouped data by columns to get summary statistics, e.g., GROUP BY billing_country.

- JOINs (INNER JOIN)
Connected multiple tables together using INNER JOIN, such as:
customer with invoice
invoice_line with track
track with genre and album

- Aliases (AS)
Renamed columns and tables for better readability, e.g., AS Total, AS RowNo.

- LIMIT Clause
Retrieved only the top results using LIMIT, such as top 1 country, top 3 invoices, etc.

- DISTINCT Keyword
Eliminated duplicate records in output using SELECT DISTINCT.

- Window Functions
Used ROW_NUMBER() to rank customers and genres per country or billing region.

- Common Table Expressions (CTEs)
Used WITH clause to write modular and readable subqueries:
popular_genre for finding most popular genre per country
Customer_with_country to get top spender per country

- Nested Queries and Subqueries
Logical structuring of complex queries to break problems into manageable parts.




