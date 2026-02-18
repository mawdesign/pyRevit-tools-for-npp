# **User Guide: Transforming Revit into an IDE with Notepad++**

This guide explains how to use the **pyRevit Tools for Notepad++** to create a high-performance "Integrated Development Environment" (IDE) for Revit content creation, based on the principles outlined in Michael Warwick's "Setting Up a Revit IDE" presentation.

## **The "IDE" Philosophy**

Standard Revit content creation often feels like "coding through a keyhole." The built-in family parameter windows and schedule views lack the bulk-editing power, search-and-replace, and syntax highlighting found in modern coding environments.

By linking Revit to **Notepad++**, we gain:

* **Global Search & Replace** across thousands of parameters.  
* **Syntax Highlighting** for complex Revit formulas.  
* **Bulk Editing** of Keynote files and Shared Parameter files.  
* **Log Analysis** with clear formatting.

## **Core Toolset Features**

### **1\. The Notepad++ Sync Tool**

Located on the **pyMAW** tab, the primary Notepad++ button acts as a contextual bridge.

* **Usage**: Click the button while in the Family Editor to instantly dump the current family's parameter data into a temporary text file in Notepad++.  
* **Why**: Use this to scan for naming inconsistencies or to copy-paste formula logic between different families without clicking through dozens of Revit dialogs.

### **2\. File Bridge (Dropdown Menu)**

The "Open..." dropdown allows you to bypass Windows Explorer and open critical Revit system files directly:

* **Keynote File**: Edit your project keynotes with full text-editing power.  
* **Shared Parameters**: Safely view and search your SPF (Shared Parameter File) without risking corruption through manual file seeking.  
* **Revit.ini & Keyboard Shortcuts**: Rapidly tweak your Revit environment settings.  
* **Current Journal**: Essential for debugging crashes; opens the latest Revit journal file for immediate review.

### **3\. Data Exporters**

The **Export** menu allows you to "extract" the logic of a Revit project for external editing:

* **Export Family Parameters**: Dumps the current family's parameter structure to a tab-separated format.  
* **Export Type Catalog**: Generates the .txt file required for type catalogs, allowing you to build hundreds of types in seconds using Notepad++'s "Column Edit" mode.  
* **Export Shared Parameters**: Extracts only the parameters currently used in the project for clean-up or migration.

### **4\. Dynamo Python Extraction**

A specialized tool for computational designers:

* **Function**: Extracts the Python code from a selected Dynamo node and opens it in Notepad++.  
* **Why**: Dynamo's built-in Python editor is notoriously small. This tool allows you to write your logic in a full-sized editor with line numbering and proper indentation.

## **Recommended Notepad++ Configuration**

To get the most out of this extension, we recommend the following Notepad++ setup:

1. **Language Customization**: Create a User Defined Language (UDL) for Revit Formulas to highlight keywords like if, and, or, not, and parameter names.  
2. **Compare Plugin**: Install the "Compare" plugin via the Notepad++ Plugins Admin. This allows you to export two different families and instantly see the differences in their parameter logic.  
3. **XML Tools**: If you work with Revit Server or BIM 360 configurations, the XML Tools plugin provides essential "Pretty Print" (indentation) features.

## **Workflow Example: Bulk Editing a Type Catalog**

1. Open your complex Revit family.  
2. Use **pyMAW \> Export \> Export Type Catalog**.  
3. In Notepad++, use **Alt \+ Shift \+ Arrow Keys** (Column Mode) to edit values across multiple rows simultaneously.  
4. Save and reload the family into Revit to see your updated types.

*This guide was developed to support the pyRevit-tools-for-npp extension. For project overview and licensing, see the [README.md](https://www.google.com/search?q=./README.md).*