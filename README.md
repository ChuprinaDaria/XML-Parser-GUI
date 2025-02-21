# XML-Parser-GUI
📂 XML to Excel Converter
This Python script extracts data from XML files and exports it to an Excel file. Using a simple Tkinter-based graphical interface, it allows users to select multiple XML files, parse specific data fields, and save the output in .xlsx format.

🔍 Features:

📁 Select multiple XML files through a graphical interface.
🔗 Extracts specific data fields:
MRN (from the filename without the prefix CC599C-)
Nr Towaru (Goods item number from the XML)
Opis Towaru (Description of the goods)
Nr Listu (Reference number from the transport document)
📊 Automatically converts the extracted data into an Excel table.
💾 Allows users to choose the save location for the output file.
⚙️ How to Use:

Install required libraries:

bash
Kopiuj
Edytuj
pip install pandas openpyxl
Run the script:

bash
Kopiuj
Edytuj
python xml_to_excel_converter.py
Follow the GUI prompts:

Select one or more XML files.
Choose where to save the Excel file.
Output:

The script will generate an Excel file (.xlsx) with the extracted data.
📚 Dependencies:

pandas for data manipulation
openpyxl for Excel file creation
xml.etree.ElementTree for XML parsing
tkinter for the graphical interface
🚀 Use Cases:

Simplifying the extraction of customs or logistics data from XML files.
Quickly converting structured XML data into a readable Excel format for analysis or reporting.
✅ Example Output:

MRN	Nr Towaru	Opis Towaru	Nr Listu
12345678	001	Electronics	AB1234567
87654321	002	Clothing	CD7654321
💡 Notes:

Make sure your XML files follow the structure expected by the script (containing GoodsItem, declarationGoodsItemNumber, descriptionOfGoods, and TransportDocument tags).
The MRN is automatically extracted from the filename, assuming it starts with the prefix CC599C-.






