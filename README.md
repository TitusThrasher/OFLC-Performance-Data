<!-- ABOUT THE PROJECT -->
## About The Project
Python script for reducing file size of public Performance Data from the U.S. Dept. of Labor's Office of Foreign Labor Certification (OFLC) for the LCA Program (H-1B, H-1B1, E-3). 

1. The script uses pandas to read an Excel file, process it, and save it as a CSV file.
2. It removes a predefined list of columns from the dataset.
3. It applies data type optimization to reduce memory usage:
  a. Object columns with less than 50% unique values are converted to categorical type.
  b. Float64 and int64 columns are downcast to the smallest possible numeric type.
4. The script prints information about the original and optimized dataset shapes and memory usage.
5. Finally, it saves the optimized dataset as a CSV file.
     
OFLC PERFORMANCE DATA SOURCE: https://www.dol.gov/agencies/eta/foreign-labor/performance

## Features

	• Column Removal: Unnecessary columns are removed from the dataset.
	• Data Type Optimization: Data types are adjusted to reduce memory usage. The script includes a function optimize_dtypes(df) that optimizes the data types in the DataFrame:
	  • Converts object types to categorical if they have less than 50% unique values.
	  • Downcasts float64 to float32 and int64 to int32 to save memory.
	• Memory Usage Reporting: The script reports memory usage before and after optimization.
	• Error Handling: The script includes error handling and logs warnings for any issues encountered during processing.

### Built With
Python 3.x
https://github.com/pandas-dev/pandas
https://github.com/numpy/numpy

## Getting Started
1.	Define File Paths: Set the 'input_excel_path' and 'output_csv_path' variables to the appropriate local file paths.
2.	Run the Script: Execute the script via terminal. The script will process the Excel file, remove unnecessary columns, optimize data types, and save the resulting dataset as a CSV fie.

## Additional Notes
	•	Error Handling: The script logs warnings for missing columns and handles errors gracefully.
	•	Memory Usage: The script provides memory usage statistics before and after optimization, helping you monitor the efficiency of the optimizations applied.
	•	Customization: You can modify the list of columns to remove or adjust the data type optimization criteria based on your specific dataset needs.

<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- CONTRIBUTING -->
## Contributing
If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License
Distributed under the MIT License. See `LICENSE.txt` for more information.


<!-- CONTACT -->
## Contact
Andrew Thrasher 
https://tituslegaldesign.com
