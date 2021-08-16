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


## Cite as

See the GLAM Workbench or [Zenodo](http://doi.org/10.5281/zenodo.3549481) for up-to-date citation details.

----

This repository is part of the [GLAM Workbench](https://glam-workbench.github.io/).  
If you think this project is worthwhile, you might like [to sponsor me on GitHub](https://github.com/sponsors/wragge?o=esb).
