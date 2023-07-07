# Installation Guide
This is a guide to installing the Python Scrapy Spider project.

## Step 1 - Clone the project
Clone the project from github:

```bash
git clone https://github.com/iAlex0/books-to-scrape.git
```

## Step 2 - Install & activate your python virtual environment
To install the python virtual environment follow the following instructions below.
`python3 -m venv venv`

Activate the new python virtual environment:
`venv/Scripts/activate`


## Step 3 - Install the required python modules
To install the required modules for this python project to run you need to install the required python modules using the following command:

`pip install -r requirements.txt`


## Step 4 - Run the project/ Follow the course
Once the required python modules are installed you should be able to view/run the Python Scrapy Spider with the following command (from within the project folder):

Cd into the project spiders: 

`cd app`

`cd bookscraper`

View the project spiders:

`scrapy list`

Run the project spider: 

`scrapy crawl bookspider`



# Helpful Dubugging 
If you have issues running the `pip install -r requirements.txt` command this can be due to some things not being up to date on your computer. 

Running the following may solve some of these issues:

`pip install --upgrade pip`

The following error: `NotADirectoryError: [Errno 20] Not a directory: 'pkg-config'` might be solvable by running:
`export PKG_CONFIG=/path/to/pkg-config`



----------------------------------------------------------------------------------------------------------------------------



# Deploy on Scrapy Cloud
To deploy the project on Scrapy Cloud you need to run the following command:

1: Create an account at  https://app.zyte.com/scrapy-cloud

2: Create a new project

3: Run the following command to deploy the project to Scrapy Cloud:

`cd app`

`pip install shub`

`shub login`

The terminal will ask for your account API_KEY which can be found at https://app.zyte.com/
- Navigate to: Settings > API Key

`API_KEY: {Enter Your API_KEY Here}`

The terminal will ask for your project ID which can be found at: app.zyte.com/p/{Enter Your Project # Here}/deploy

`shub deploy {Enter Your Project # Here}`


## License
MIT © iAlex0