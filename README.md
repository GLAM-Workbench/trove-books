# Trove books

Here you'll find Jupyter notebooks to work with data from Trove's 'book' zone. Trove's 'book' zone includes books (of course), but also ephemera (like pamphlets and leaflets) and theses. You can access metadata from the book zone through the Trove API.

See the [Trove books section](https://glam-workbench.net/trove-books/) of the GLAM Workbench for more details.

## Notebook topics

### Harvesting data

* [**Harvesting the text of digitised books (and ephemera)**](Harvesting-digitised-books.ipynb) – assemble a list of books in digital form using the API, then download OCRd text from as many as possible
* [**Metadata for Trove digitised works**](Metadata-for-Trove-digitised-works.ipynb) – extract embedded metadata from digital work pages
* [**Getting the text of Trove books from the Internet Archive**](Getting-Trove-books-from-Internet-Archive.ipynb) – identify books in Trove that are available through the Internet Archive, download text where available


### Exploring harvested books

* [**Counting words and phrases**](counting-words-in-text.ipynb) – simple examples of counting words and ngrams in a piece of text, using OCRd text from Trove books
* [**Recipe generator**](recipe-generator.ipynb) – extracts parts of speech from the OCRd text of a recipe book available through Trove, then reassemble to create random recipes
* **[Exploring the Digitised Books Collection from Trove](https://nbviewer.jupyter.org/github/adelr/trove-books/blob/master/Trove_Digitised_Books)** by  [Adel Rahmani](https://twitter.com/dinkumdata)**

## Data downloads

* **OCRd text from Trove books and ephemera (harvested August 2021)** – [browse the full collection in CloudStor](https://cloudstor.aarnet.edu.au/plus/s/ugiw3gdijSKaoTL) or [explore using a searchable database](https://trove-digital-books.glitch.me/data/trove-digital-books) hosted on Glitch
* **CSV formatted list of books with OCRd text** – [download CSV file](https://github.com/GLAM-Workbench/trove-books/blob/master/trove_digitised_books_with_ocr.csv) or [explore using a searchable database](https://trove-digital-books.glitch.me/data/trove-digital-books) hosted on Glitch
* **OCRd text from the Internet Archive of 'Australian' books listed in Trove** – [browse the collection in CloudStor](https://cloudstor.aarnet.edu.au/plus/s/3h3GHfS3tQTDLaX)
* **CSV formatted list of 'Australian' books in Trove with full text versions in the Internet Archive – download CSV file** – [download the CSV file](https://github.com/GLAM-Workbench/trove-books/blob/master/trove-books-in-ia.csv)

<!-- START RUN INFO -->

## Run these notebooks

There are a number of different ways to use these notebooks. Binder is quickest and easiest, but it doesn't save your data. I've listed the options below from easiest to most complicated (requiring more technical knowledge).

### Using Binder

[![Launch on Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GLAM-Workbench/trove-books/master/?urlpath=lab/tree/index.md)

Click on the button above to launch the notebooks in this repository using the [Binder](https://mybinder.org/) service (it might take a little while to load). This is a free service, but note that sessions will close if you stop using the notebooks, and no data will be saved. Make sure you download any changed notebooks or harvested data that you want to save.

See the [Using Binder](https://glam-workbench.net/using-binder/) section of the GLAM Workbench for more details.

### Using Reclaim Cloud

[![Launch on Reclaim Cloud](https://glam-workbench.github.io/images/launch-on-reclaim-cloud.svg)](https://app.my.reclaim.cloud/?manifest=https://raw.githubusercontent.com/GLAM-Workbench/trove-books/master/reclaim-manifest.jps)

[Reclaim Cloud](https://reclaim.cloud/) is a paid hosting service, aimed particularly at supported digital scholarship in hte humanities. Unlike Binder, the environments you create on Reclaim Cloud will save your data – even if you switch them off! To run this repository on Reclaim Cloud for the first time:

* Create a [Reclaim Cloud](https://reclaim.cloud/) account and log in.
* Click on the button above to start the installation process.
* A dialogue box will ask you to set a password, this is used to limit access to your Jupyter installation.
* Sit back and wait for the installation to complete!
* Once the installation is finished click on the 'Open in Browser' button of your newly created environment (note that you might need to wait a few minutes before everything is ready).

See the [Using Reclaim Cloud](https://glam-workbench.net/using-reclaim-cloud/) section GLAM Workbench [for more details.

### Using Docker

You can use Docker to run a pre-built computing environment on your own computer. It will set up everything you need to run the notebooks in this repository. This is free, but requires more technical knowledge – you'll have to install Docker on your computer, and be able to use the command line.

* Install [Docker Desktop](https://docs.docker.com/get-docker/).
* Create a new directory for this repository and open it from the command line.
* From the command line, run the following command:  
  ```
  docker run -p 8888:8888 --name trove-books -v "$PWD":/home/jovyan/work glamworkbench/trove-books repo2docker-entrypoint jupyter lab --ip 0.0.0.0 --NotebookApp.token='' --LabApp.default_url='/lab/tree/index.md'
  ```
* It will take a while to download and configure the Docker image. Once it's ready you'll see a message saying that Jupyter Notebook is running.
* Point your web browser to `http://127.0.0.1:8888`

See the [Using Docker](https://glam-workbench.net/using-docker/) section of the GLAM Workbench for more details.

### Setting up on your own computer

If you know your way around the command line and are comfortable installing software, you might want to set up your own computer to run these notebooks.

Assuming you have recent versions of Python and Git installed, the steps might be something like:

* Create a virtual environment, eg: `python -m venv trove-books`
* Open the new directory" `cd trove-books`
* Activate the environment `source bin/activate`
* Clone the repository: `git clone https://github.com/GLAM-Workbench/trove-books.git notebooks`
* Open the new `notebooks` directory: `cd notebooks`
* Install the necessary Python packages: `pip install -r requirements.txt`
* Run Jupyter: `jupyter lab`

See the GLAM Workbench for more details.

<!-- END RUN INFO -->

## Cite as

See the GLAM Workbench or [Zenodo](http://doi.org/10.5281/zenodo.3549481) for up-to-date citation details.

----

This repository is part of the [GLAM Workbench](https://glam-workbench.github.io/).  
If you think this project is worthwhile, you might like [to sponsor me on GitHub](https://github.com/sponsors/wragge?o=esb).
