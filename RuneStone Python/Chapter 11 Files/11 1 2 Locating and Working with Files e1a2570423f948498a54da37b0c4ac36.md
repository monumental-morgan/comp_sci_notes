# 11.1/2 Locating and Working with Files

# 11.1 Working With Data Files

- In Python, we must **open** files before we can use them and **close** them when we are done with them
- Once a file is opened it becomes a Python object just like all other data

![https://remnote-user-data.s3.amazonaws.com/Z7CQFt9ftVXHbt6nw3zccEQ5j9mtdtCRGPYxjA8qMTQw9zgOri_HrO3NruFj5SQVj5ihXEd8yNslVR5B2xO5q3074lf5BbQtnt_echlo1aWbImTPeTNZL9D6xkHn38sX.png](https://remnote-user-data.s3.amazonaws.com/Z7CQFt9ftVXHbt6nw3zccEQ5j9mtdtCRGPYxjA8qMTQw9zgOri_HrO3NruFj5SQVj5ihXEd8yNslVR5B2xO5q3074lf5BbQtnt_echlo1aWbImTPeTNZL9D6xkHn38sX.png)

# 11.2 Finding a File on your Disk

![https://remnote-user-data.s3.amazonaws.com/pZLOYtdtQhLl-6JAnt3CTZ8OpDq3xziCdbbeGZTXbji4cbub3oBdyj_2bRSnrmcrm15Sr7RFJnybBVQDDbWZ5MgZ4Nt_RXWwoaEmLnVa050CWJGuBG2sNn25YlwN9h_e.png](https://remnote-user-data.s3.amazonaws.com/pZLOYtdtQhLl-6JAnt3CTZ8OpDq3xziCdbbeGZTXbji4cbub3oBdyj_2bRSnrmcrm15Sr7RFJnybBVQDDbWZ5MgZ4Nt_RXWwoaEmLnVa050CWJGuBG2sNn25YlwN9h_e.png)

- Here’s the important rule to remember: If your file and your Python program are in the same directory you can simply use the filename like this: `open('myfile.txt', 'r')`
- If your file and your Python program are in different directories then you must refer to one or more directories:
    - in a *relative file path* to the file like this: `open('../myData/data3.txt', 'r')`
    - or in an *absolute file path* like `open('/users/bmiller/myFiles/allProjects/myData/data3.txt', 'r')`