# Topic 10: File Handling

In this topic, we'll explore file handling in Python, which allows us to read and write data to external files. File handling is essential for processing data, storing configurations, and interacting with the external world.

Items covered:

  ## Opening and Closing Files:
          Python provides the open() function to open files in different modes (read, write, append, etc.).
          It's essential to close files after use to free up system resources.
          Syntax to open a file:
  
          python
  
  file = open("filename.txt", "mode")
  
  Syntax to close a file:
  
  python
  
      file.close()

## Reading from Files:

      The read() method reads the entire content of a file as a string.
      The readline() method reads one line at a time.
      The readlines() method reads all lines and returns a list of lines.
      Example:
  
      python
  
      with open("data.txt", "r") as file:
          content = file.read()
          print(content)

## Writing to Files:
    
        The write() method writes data to a file, overwriting the existing content.
        The writelines() method writes a list of strings to a file.
        Use mode "w" or "a" for writing or appending to a file, respectively.
        Example:
    
        python
    
        with open("output.txt", "w") as file:
            file.write("Hello, this is a new file.")

## Handling CSV Files:

        Python's csv module allows easy handling of CSV (Comma Separated Values) files.
        You can read CSV files using the csv.reader() function and write them with the csv.writer() function.
        Example:
    
        python
    
        import csv
    
        with open("data.csv", "r") as file:
            csv_reader = csv.reader(file)
            for row in csv_reader:
                print(row)

## Handling JSON Files:

        JSON (JavaScript Object Notation) is a popular data interchange format.
        Python's json module allows easy handling of JSON files.
        You can read JSON files using the json.load() function and write them with the json.dump() function.
        Example:
    
        python
    
            import json
    
            data = {"name": "John", "age": 25}
    
            with open("data.json", "w") as file:
                json.dump(data, file)
    
## Summary: 
    File handling is a crucial aspect of data manipulation and storage in Python. 
    It enables you to read data from external sources, process it, and store results for later use. 
    Practice working with files to gain confidence in handling real-world data.
