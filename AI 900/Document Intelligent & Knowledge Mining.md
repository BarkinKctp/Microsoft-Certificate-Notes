## DOCUMENT INTELLIGENT

### Azure AI Document Intelligent

- **Prebuilt Models**  
  The prebuilt models apply advanced machine learning to accurately identify and extract text, key-value pairs, tables, and structures from forms and documents.

- **Custom Models**  
  Custom models can be trained to identify specific fields that are not included in the existing pretrained models.

- **Document Analysis**  
  General document analysis that returns structured data representations, including regions of interest and their inter-relationships.

---

## PREBUILT MODELS

The model has been trained to recognize several different languages, depending on the receipt type.  
For best results when using the prebuilt receipt model, images should be:

- JPEG, PNG, BMP, PDF, or TIFF format  
- File size less than 500 MB for paid (S0) tier and 4 MB for free (F0) tier  
- Between 50 x 50 pixels and 10000 x 10000 pixels  
- For PDF documents, no larger than 17 inches x 17 inches  
- One receipt per document  

---

## KNOWLEDGE MINING AND AI SEARCH

### Azure AI Search

- **Data from any source**: accepts data from any source provided in JSON format, with auto crawling support for selected data sources in Azure.
- **Multiple options for search and analysis**: including vector search, full text, and hybrid search.
- **AI enrichment**: has Azure AI capabilities built in for image and text analysis from raw content.
- **Linguistic analysis**: offers analysis for 56 languages to intelligently handle phonetic matching or language-specific linguistics. Natural language processors available in Azure AI Search are also used by Bing and Office.
- **Configurable user experience**: has options for query syntax including vector queries, text search, hybrid queries, fuzzy search, autocomplete, geo-search filtering based on proximity to a physical location, and more.
- **Azure scale, security, and integration**: at the data layer, machine learning layer, and with Azure AI services and Azure OpenAI.

An **indexer** serializes a source document into JSON before passing it to a search engine for indexing.  
An indexer automates several steps of data ingestion, reducing the amount of code you need to write.

---

=========================================================================

**Invoice model** extracts key information from sales invoices and is suitable for extracting information from sales account documents.

**ID document model** is optimized to analyze and extract key information from US driver’s licenses and international passport biographical pages.

**Business card model** analyzes and extracts key information from business card images and includes common data field extractions, such as name and email.

**Receipt model**

**Language model**

---
