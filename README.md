# 🇵🇱 Web Scraping — Poland Facilities

This repository contains web scraping and data extraction work developed during my **previous professional experience in Poland**.

The project focused on collecting, cleaning, and structuring publicly available information about **sports facilities, schools, public courts, and recreational infrastructure across several Polish cities**.

## Project Context

During my previous experience in Poland, I worked on gathering facility-related data from multiple public sources.

The objective was to transform fragmented and unstructured web data into structured datasets that could be used for further analysis, mapping, enrichment, or integration into other data workflows.

The work covered several locations in Poland, including:

- Kraków
- Warsaw
- Wrocław
- Sopot
- Gdańsk
- Gdynia
- Trójmiasto area

Depending on the source, the collected information included:

- Facility name
- Address
- City
- Postal code
- Phone number
- Website
- Email
- Facility type
- Available sports courts
- Activities
- Geographic coordinates
- School and public infrastructure information

---

## Project Notebooks

### `scrap_Krakaw.ipynb`

Web scraping workflow for sports and recreational facilities in **Kraków**.

The notebook includes:

- Facility URL collection with Selenium
- HTTP requests to individual facility pages
- HTML parsing with BeautifulSoup
- Contact information extraction
- Sports facility and activity extraction
- Data cleaning using regular expressions
- Data structuring with Pandas

Typical extracted fields:

```text id="rkp12a"
name
address
telephone
email
website
courts
activities
```

---

### `Scraping_Public_Court_Warsaw.ipynb`

Collection and processing of information related to **public sports courts and facilities in Warsaw**.

The purpose was to transform publicly available facility information into structured data that could be reused in broader datasets and analysis workflows.

---

### `Scraping_Sopot_schools.ipynb`

Data extraction related to **schools and associated infrastructure in Sopot**.

This notebook focuses on collecting and structuring information about educational facilities and their associated infrastructure.

---

### `Map_scholl_worclow.ipynb`

Processing of sports and school facility data for **Wrocław**.

This part of the work also involved geographic data and KML processing.

Example fields:

```text id="kml983"
Facility.Name
Facility.Adress
Facility.Courts
```

The notebook extracts and cleans facility descriptions, addresses, and geographic information.

---

### `BS scraping katalog.trojmiasto.ipynb`

Web scraping and data processing for facilities in the **Trójmiasto area**, mainly covering Gdańsk, Gdynia, and Sopot.

Example resulting fields:

```text id="troj321"
name
streetAddress
postalCode
cityID
cityName
userTel
userWeb
category
listActivities
```

The collected data includes different categories of sports, health, fitness, and recreational facilities.

---

## Technologies Used

The project was developed mainly with **Python and Jupyter Notebook**.

Technologies and libraries used include:

- Python
- Pandas
- Selenium
- BeautifulSoup
- Requests
- Regular Expressions
- PyKML
- lxml
- tqdm
- Jupyter Notebook

---

## Data Collection Workflow

The general workflow used across the different sources was:

```text id="flow764"
Public Web Sources
        ↓
Selenium / Requests
        ↓
HTML / KML Extraction
        ↓
BeautifulSoup / PyKML
        ↓
Data Cleaning
        ↓
Regex Processing
        ↓
Pandas
        ↓
Structured Dataset
```

---

## Technical Challenges

Working with multiple independent public data sources required handling several practical challenges:

- Different HTML structures across websites
- Inconsistent field formats
- Missing information
- Dynamic web content
- Multiple page layouts
- Data duplication
- Cleaning unstructured text
- Extracting information from geographic/KML sources
- Standardizing data coming from different cities

A significant part of the work consisted of building extraction and cleaning logic adapted to each source.

---

## Skills Demonstrated

This project reflects practical experience with:

- Web scraping
- Browser automation
- Data extraction
- HTML parsing
- Data cleaning
- Data transformation
- Regular expressions
- Pandas
- Geographic data processing
- KML parsing
- Working with heterogeneous data sources
- Structuring unstructured web data

---

## Geographic Coverage

```text id="geo471"
Poland
├── Kraków
├── Warsaw
├── Wrocław
├── Sopot
├── Gdańsk
└── Gdynia
```

---

## Note

This repository contains work from a **previous professional experience in Poland** and is published primarily to showcase the technical approaches and data engineering/web scraping work involved.

Because the notebooks rely on external websites, some selectors, URLs, or scraping logic may no longer work exactly as originally implemented if the source websites have changed.

---

## Author

**Med Seddik**

GitHub: [@medseddik1999](https://github.com/medseddik1999)
