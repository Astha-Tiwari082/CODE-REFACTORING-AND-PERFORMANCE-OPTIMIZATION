# CODE REFACTORING AND PERFORMANCE OPTIMIZATION

*COMAPNY*: CODTECH IT SOLUTIONS

*NAME*: ASTHA TIWARI

*INTERN ID*: CT06DF1961

*DOMAIN*: SOFTWARE DEVELOPMENT

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH 

# CODE REFACTORING AND PERFORMANCE OPTIMIZATION PROJECT DESCRIPTION
The task of code refactoring and performance optimization involves selecting an existing piece of software—typically an open-source or legacy codebase—and improving its internal structure without altering its external behavior. In this specific exercise, a Java class named FundingRaised was chosen, which is responsible for reading and filtering records from a CSV file containing startup funding data. The class initially performed its core functions but was written in a way that lacked modularity, was difficult to maintain, and did not easily support enhancements or scale to accommodate larger data operations. The goal of this task was to improve the readability, maintainability, and structural clarity of the code while preserving its original functionality and ensuring that any performance-related concerns were addressed appropriately.
The development work was carried out using IntelliJ IDEA Community Edition, a popular integrated development environment that offers powerful static code analysis, debugging tools, and developer productivity features. The programming language used was Java 8, which is still widely supported in enterprise environments. The OpenCSV library was utilized for parsing CSV files, allowing the code to read structured data rows efficiently. Version control was handled with Git, which tracked incremental changes, making it easier to compare before and after versions of the code and revert or merge changes when necessary. Testing was done manually using a simple main method and IntelliJ’s built-in console and debugger tools to verify correctness at each step.
One of the main motivations behind this task was to demonstrate how code that initially works can still be a liability in larger systems due to poor design. The original version of the FundingRaised class had multiple blocks of redundant logic. It accessed CSV columns using hardcoded index values, which made the code fragile in case the CSV schema changed. Filtering was implemented in a way that was verbose and repetitive, with separate loops and conditions for each potential filter like company name, city, state, and funding round. Exception handling was minimal and uninformative, which could pose challenges during debugging or when the code is integrated into a larger system.
By refactoring the class, the codebase was significantly improved. A centralized method for reading CSV data was introduced to eliminate repetition. A static array of headers was defined and used to dynamically map each CSV row into a structured format using maps. Filtering logic was consolidated into a single reusable function that checks whether a row matches all specified criteria. Exception messages were enhanced to provide better context, and the output of the main method was improved for more effective manual testing. These changes not only made the code easier to read but also made it more scalable and adaptable to new requirements in the future.
This type of task is widely applicable in the real world. Software developers frequently work with existing codebases that need to be cleaned up for better performance, reliability, and readability. Whether maintaining an internal business tool, contributing to open-source projects, or building data processing pipelines, the ability to refactor and optimize code is an essential skill. It helps reduce technical debt, improves collaboration, and sets the stage for future development and integration work.
