# Spotify_Data_Analysis_SQL

![image](https://github.com/user-attachments/assets/4bf33359-ddd0-4723-89e0-8af9fcdb4879)

## 📑 Contents

- [**Introduction**](#introduction)
- [**💾 Data Setup in SQL Workbench**](#-data-setup-in-sql-workbench)
- [**🔍 Exploring the Dataset**](#-exploring-the-dataset)
- [**SQL Concepts Used**](#sql-concepts-used)
- [**Data Source**](#data-source)
- [**Key Insights**](#key-insights)
- [**Skills Gained**](#skills-gained)
- [**Future Scope**](#future-scope)

The Spotify Data Analysis Project: In today's changing world, data analysis has become crucial in fields such as business, research, and meteorology. This project showcases the role that data plays in making decisions, advancing research initiatives, and even predicting weather patterns.

The immense potential of data analysis is evident in this project, which focuses on extracting insights from music-related datasets using SQL queries and aggregate functions (Sum, Order by, Group by, Rank, Limit,  etc.). At its core, Spotify takes center stage as an audio streaming giant with captivating features like seamless song sharing and synchronized lyrics display.

Throughout this project, I delved into the realm of data using SQL’s built-in functions and JOIN operations. From analyzing to visualizing the data , this project covers all aspects of data processing. The interactive environment provided by SQL editor as MySQL Workbench enhanced my experience by allowing me to engage with the data and discover patterns.

Through the Spotify Data Analysis Project, I not only sharpened my SQL querying skills but also gained a deep understanding of how data intertwines with the world of music. This journey provided insights and equipped me with confidence to undertake similar projects in the future.

Don't forget to follow and star ⭐ the repository if you find it valuable.

Tools Used🛠️:
My Sql Workbench

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
select * from album;
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






