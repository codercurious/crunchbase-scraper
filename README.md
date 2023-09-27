[Demo video](https://www.youtube.com/watch?v=WHMA9wB-lWY)


Crunchbase is a platform where you can discover innovative companies, connect with the people behind them, and uncover new opportunities. It has become a prime source of business information for millions of users around the world.

### **Importance of Crunchbase Data**

Data from Crunchbase is highly sought after. It can provide invaluable insights about startups, their funding rounds, key individuals involved, and much more. Therefore, scraping this data can equip businesses with information necessary for decision-making and strategy development.

### **Why Apify for Crunchbase Data Scraping?**

Apify is a web scraping and automation platform. It allows you to extract data, automate workflows, and integrate with your existing software. It's flexible, easy to use, and scalable, making it a top choice for many businesses.

### **Crunchbase Data Scraper: The Apify Actor**

Crunchbase Data Scraper is a specific Apify actor that focuses on retrieving data from Crunchbase.

#### **How Does It Work?**

This actor is programmed to navigate through the Crunchbase's complex website structure, find the relevant data, and extract it in a structured, usable format.

#### **Features of the Crunchbase Data Scraper**

The Crunchbase Data Scraper actor offers features such as being able to extract company profiles, key person profiles, funding rounds, acquisitions, and more. It provides a lot of flexibility, allowing you to specify what data you want.

#### **Use Cases**

Crunchbase Data Scraper is highly beneficial for market researchers, sales teams, data analysts, and more. It helps streamline various processes, from lead generation to industry analysis.


### Sample output data for company search results

```json

{
	"uuid": "e36f580e-6c0e-47de-accf-15de75f62cc9",
	"name": "Stability AI",
	"type": "organization",
	"imageUrl": "https://res.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_25,w_25,f_auto,b_white,q_auto:eco,dpr_1/yngvetlwqatjdqwmxg9g",
	"link": "https://www.crunchbase.com/organization/stability-ai",
	"numberOfEmployees": [
		51,
		100
	],
	"website": {
		"value": "https://stability.ai"
	},
	"linkedin": {
		"value": "https://www.linkedin.com/company/stability-ai"
	},
	"short_description": "Stability AI is an artificial intelligence-driven visual art startup that designs and implements open AI tools.",
	"categories": [
		{
			"entity_def_id": "category",
			"permalink": "artificial-intelligence",
			"uuid": "c4d8caf3-5fe7-359b-f9f2-2d708378e4ee",
			"value": "Artificial Intelligence"
		},
		{
			"entity_def_id": "category",
			"permalink": "image-recognition",
			"uuid": "af9307c9-6413-72ae-aac7-4391df240dd2",
			"value": "Image Recognition"
		},
		{
			"entity_def_id": "category",
			"permalink": "information-technology-dbca",
			"uuid": "dbca89fa-f083-5438-b4ad-d3fdeceb78e7",
			"value": "Information Technology"
		},
		{
			"entity_def_id": "category",
			"permalink": "software",
			"uuid": "c08b5441-a05b-9777-b7a6-012728caddd9",
			"value": "Software"
		}
	],
	"location_identifiers": [
		{
			"permalink": "london-england",
			"uuid": "aad17950-576b-8c44-8fd4-f44dbeb59220",
			"location_type": "city",
			"entity_def_id": "location",
			"value": "London"
		},
		{
			"permalink": "england-united-kingdom",
			"uuid": "79eb923b-9e93-e0db-2fe0-75f0c430c2cb",
			"location_type": "region",
			"entity_def_id": "location",
			"value": "England"
		},
		{
			"permalink": "united-kingdom",
			"uuid": "a30e342c-1742-6b1c-66e9-461de680e54b",
			"location_type": "country",
			"entity_def_id": "location",
			"value": "United Kingdom"
		},
		{
			"permalink": "europe",
			"uuid": "6106f5dc-823e-5da8-40d7-51612c0b2c4e",
			"location_type": "continent",
			"entity_def_id": "location",
			"value": "Europe"
		}
	],
	"twitter": {
		"value": "https://www.twitter.com/stabilityai"
	},
	"contact_email": "info@stability.ai",
	"rank_org_company": 40
}

```

### Documentation

This JSON data represents companies as a result of a search performed in the Crunchbase database.

Here are the descriptions for each field in the JSON data:

- `uuid`: The unique identifier for the company in the database. Each `uuid` is a string following the standard UUID format.
- `name`: The official name of the company.
- `type`: This field indicates the type of the entry. For this particular entry, the type is 'organization'.
- `imageUrl`: URL of the company's logo or relevant image.
- `link`: The direct link to the company's profile on Crunchbase.
- `numberOfEmployees`: An array indicating the range of the company's employee count.
- `website`: An object that contains the `value` field which provides the company's official website URL.
- `linkedin`: An object that contains the `value` field which provides the LinkedIn profile URL of the company.
- `short_description`: A brief description of the company and its primary functions or industry.
- `categories`: An array of category objects that the company falls under. Each object in the array has the following fields:
    - `entity_def_id`: The identifier of the category entity.
    - `permalink`: A URL-friendly version of the category name.
    - `uuid`: The unique identifier for the category.
    - `value`: The actual name of the category.
- `location_identifiers`: An array of location objects that correspond to the company's location. Each object in the array has the following fields:
    - `permalink`: A URL-friendly version of the location name.
    - `uuid`: The unique identifier for the location.
    - `location_type`: The type of the location. It could be 'city', 'region', 'country', or 'continent'.
    - `entity_def_id`: The identifier of the location entity.
    - `value`: The actual name of the location.
- `twitter`: An object that contains the `value` field which provides the Twitter profile URL of the company.
- `contact_email`: The contact email address for the company.
- `rank_org_company`: The company's rank among other companies in the Crunchbase database.

The structure of this JSON data makes it easy to parse and use in various applications, such as website scrapers, data analysis tools, and so on. Remember, however, to respect the data usage terms and conditions of Crunchbase when using their data.
