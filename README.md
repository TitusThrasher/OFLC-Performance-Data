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

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With
https://github.com/pandas-dev/pandas

[https://github.com
](https://github.com/numpy/numpy)

<!-- GETTING STARTED -->
## Getting Started
To get a local copy up and running, 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage






<!-- CONTRIBUTING -->
## Contributing
If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

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
