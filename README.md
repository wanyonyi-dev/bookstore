# XML Bookstore Project

This project demonstrates the implementation of a simple bookstore catalog system using XML technologies including DTD, XML Schema, and dynamic web display.

## 📚 Project Overview

The project consists of a bookstore catalog system that:
- Stores book information in XML format
- Validates data using both DTD and XML Schema
- Displays the catalog in a web browser with a clean, tabular format

## 🗂 Project Structure

```
bookstore/
├── README.md
├── index.html              # Main viewer page
├── bookstore.xml          # XML data file
├── bookstore.dtd          # Document Type Definition
├── bookstore.xsd          # XML Schema Definition
└── bookstore.xslt         # XSLT Stylesheet (optional)
```

## 📋 File Descriptions

### bookstore.xml
Contains the actual book data in XML format. Each book entry includes:
- Title
- Author
- Price
- ISBN
- Category
- Publication Year

### bookstore.dtd
Defines the structure and rules for the XML document, including:
- Required elements
- Element hierarchy
- Allowed attributes
- Data type constraints

### bookstore.xsd
Provides more detailed validation rules including:
- Precise data types
- Value restrictions
- Complex type definitions
- Attribute rules

### index.html
Displays the bookstore catalog in a web browser with:
- Responsive table layout
- Styled presentation
- Dynamic XML loading and parsing

## 🚀 Setup and Running

1. **Prerequisites**
   - Web browser (Chrome, Firefox, etc.)
   - Python (for running local server) or any other local server solution

2. **Installation**
   ```bash
   # Clone or download the project files
   # Create a new directory
   mkdir bookstore
   # Copy all project files into the directory
   ```

3. **Running the Project**
   ```bash
   # Navigate to project directory
   cd bookstore
   
   # Start local server using Python 3
   python -m http.server 8000
   
   # OR using Python 2
   python -m SimpleHTTPServer 8000
   ```

4. **Access the Project**
   - Open your web browser
   - Navigate to: `http://localhost:8000`

## 💡 Usage

### Adding New Books
To add new books to the catalog, edit the `bookstore.xml` file:
```xml
<book category="fiction">
    <title>Book Title</title>
    <author>Author Name</author>
    <price>29.99</price>
    <isbn>978-1234567890</isbn>
    <category>fiction</category>
    <publication_year>2024</publication_year>
</book>
```

### Validation
To validate your XML:
1. **DTD Validation**
   - The XML file automatically validates against DTD when loaded
   - Check browser console for any validation errors

2. **Schema Validation**
   - Use online validators like [xmlvalidation.com](https://www.xmlvalidation.com/)
   - Or use XML editors with validation capabilities

## 🔧 Troubleshooting

Common issues and solutions:

1. **Blank Page in Browser**
   - Ensure you're accessing via local server (http://localhost:8000)
   - Check browser console for errors
   - Verify all files are in the correct directory

2. **XML Validation Errors**
   - Verify XML syntax is correct
   - Check that all required elements are present
   - Ensure category attributes match allowed values

3. **Display Issues**
   - Clear browser cache
   - Try a different browser
   - Check file permissions

## 📝 Notes

- The project uses client-side JavaScript to parse and display XML data
- All styling is contained within index.html for simplicity
- The system supports three book categories: children, fiction, and non-fiction

## 🤝 Contributing

To contribute to this project:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Support

For support and questions:
- Create an issue in the repository
- Contact the project maintainer
- Check documentation for common solutions

## ✨ Future Enhancements

Planned features for future versions:
- Search functionality
- Sorting capabilities
- Filter by category
- Export to PDF
- Print-friendly version
