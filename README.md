### **README: Web Scraping and Text Analysis of Martin Luther King Jr.'s Speech**

---

## **Project Overview**

This project demonstrates how to use Python for **web scraping**, **text preprocessing**, and **word frequency analysis**. The goal is to extract Martin Luther King Jr.'s speech from a webpage, clean and process the text, and analyze word frequencies. The results are exported as a **CSV file** for further analysis or visualization.

---

## **Technologies Used**

- **Python 3.x**
- **BeautifulSoup**: For parsing and extracting data from HTML.
- **Requests**: For fetching web page content.
- **re (Regular Expressions)**: For text pattern matching and cleaning.
- **pandas**: For data manipulation and analysis.

---

## **Project Workflow**

### **1. Web Scraping**
- The speech text is extracted from a webpage using the `requests` library.
- The HTML content is parsed with `BeautifulSoup`.
- All `<p>` tags containing speech text are collected.

### **2. Text Preprocessing**
- Paragraphs are joined into a single string.
- Carriage returns and newlines are replaced with spaces.
- Punctuation is removed using regular expressions.
- Text is converted to lowercase for uniformity.
- Words are tokenized using whitespace as a delimiter.

### **3. Word Frequency Analysis**
- Words are counted and sorted using a `pandas` DataFrame.
- Word frequencies are calculated.

### **4. Data Export**
- The resulting word count data is saved to a CSV file:
  ```
  Web Scraper + Regular Expression Project/mlk_speech_counts.csv
  ```
- Columns:
   - **Word:** The unique word from the speech.
   - **Counts:** The frequency of that word.

---

## **Installation**

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/mlk-speech-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mlk-speech-analysis
   ```
3. Install required dependencies:
   ```bash
   pip install beautifulsoup4 requests pandas
   ```

---

## **Usage**

1. Run the script:
   ```bash
   python script.py
   ```
2. The resulting CSV file (`mlk_speech_counts.csv`) will be saved in:
   ```
   Web Scraper + Regular Expression Project/
   ```

---

## **File Structure**

```
├── script.py          # Main Python script
├── requirements.txt   # List of dependencies
├── Web Scraper + Regular Expression Project/
│   ├── mlk_speech_counts.csv  # Output word count data
└── README.md          # Project documentation
```

---

## **Results Example**

| Word       | Counts |
|------------|--------|
| freedom    | 20     |
| justice    | 15     |
| dream      | 12     |
| together   | 10     |

---

## **Future Improvements**
- Include data visualizations (e.g., word clouds, bar charts).
- Add support for analyzing multiple speeches.
- Implement a user interface for inputting URLs dynamically.

---


Happy Analyzing! 🚀
