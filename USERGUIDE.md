# **User Guide: Transforming Revit into an IDE with Notepad++**

This guide explains how to use the **pyRevit Tools for Notepad++** to create a high-performance "Integrated Development Environment" (IDE) for Revit content creation, based on the principles outlined in Michael Warwick's "Setting Up a Revit IDE" presentation from BiLT ANZ 2024.

## **The "IDE" Philosophy**

Standard Revit content creation often feels like "coding through a keyhole." The built-in family parameter windows and schedule views lack the bulk-editing power, search-and-replace, and syntax highlighting found in modern coding environments.

By linking Revit to **Notepad++**, we gain:

* **Global Search & Replace** across many parameters.  
* **Syntax Highlighting** for complex Revit formulas.  
* **Bulk Editing**, and easy access to various Revit confige files, Keynote files, and Shared Parameter files.  
* **Log Analysis** with clear formatting.

## **Core Toolset Features**

### **1\. The Open Notepad++ Button**

![Screenshot of pyMAW Notepad++ ribbon](/images/toolbar.png)\
Located on the **pyMAW** tab, the primary Notepad++ button simply opens Notepad++, shift-click to configure the location of Notepad++.

### **2\. The Notepad++ Open Tools**

![Screenshot of pyMAW Notepad++ ribbon](/images/opendropdown.png)\
This drop down contains tools that **open** most of the ancillary files Revit uses, they find the right one for the version of Revit that 
you are using and related to your username, and tell Notepad++ what language to use to for syntax highlighting for readability. Gives you 
quick access without having to search the web for the file location, because the Revit support files are in all sorts of places.

### **3\. Export to Notepad++ Tools**

![Screenshot of pyMAW Notepad++ ribbon](/images/exportdropdown.png)\
This drop-down contains tools that **export** data from Revit to Notepad++, for example there are tools to create a shared parameter, hatch, 
or keynote file from a project. These tools generally try to export in a format that is useful, so instead of just a data dump you get a 
formatted file. As an example, the keynote export creates a keynote file you can immediately link into a project. The Revit Server and Cloud 
Cache exports create draft batch scripts you can use to work with these files. These are the most powerful functions in this set of tools.

### **4\. Dynamo Python Extraction**

![Screenshot of pyMAW Notepad++ ribbon](/images/dynamo.png)\
Extracts the Python scripts from any Dynamo graph you have. This overcomes the limitation of only having one Dynamo graph open at a time, for 
example when you know that you have written a similar one before. By opening the scripts in Notepad++ you can copy and paste without closing 
the graph in Dynamo. Better still if you download the excellent aussieBIMguru or Sol Amour Dynamo libraries then all that embedded Python 
goodness is quickly accessible.

## **Recommended Notepad++ Configuration**

To get the most out of this extension, we recommend installing the companion Notepad++ PythonScript tools from https://github.com/mawdesign/RevitToolsForNotepadpp

## **Workflow Example: Bulk Editing a Type Catalog**

![Screenshot of pyMAW Notepad++ ribbon](/images/workflow.png)\
1. Open your complex Revit family.  
2. Use **pyMAW \> Export \> Export Family Parameters**.  
3. In Notepad++, use **Plugins \> PythonScript \> Scripts \> RevitFormulasForEverydayUse** to add a formula to select the max value from 4 parameters
4. Select the new formula and use **Plugins \> PythonScript \> Scripts \> RevitFormulaReformat** to create an indented view of the nested if statements and clearly
   see the structure of the formula.
5. Use **Plugins \> PythonScript \> Scripts \> RevitFormulaReformatUndo** to turn the formula back into a single line for cut-and-paste back into the Revit
   Family Parameters editor.

*This guide was developed to support the pyRevit-tools-for-npp extension. For project overview and licensing, see the [README.md](https://www.google.com/search?q=./README.md).*
