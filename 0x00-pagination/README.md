# Pagination Project

## Author
**Harrison Eze**  
GitHub: [harystyleseze](https://github.com/harystyleseze)

## Description
This project implements a pagination system for a dataset containing popular baby names. The primary goal is to efficiently manage and navigate through large datasets using pagination techniques, ensuring performance and usability even in cases where data may be deleted or modified.

### Features
- **Simple Pagination**: Basic pagination functionality to return specific pages of data.
- **Hypermedia Pagination**: Enhanced pagination that includes metadata about the current page and links to next and previous pages.
- **Deletion-Resilient Hypermedia Pagination**: A robust pagination system that accounts for potential deletions in the dataset, ensuring that users can still access the intended data without encountering gaps.

## Directory Structure
```
0x00-pagination/
│
├── 0-simple_helper_function.py  # Helper function for index range calculation
├── 1-simple_pagination.py        # Simple pagination implementation
├── 2-hypermedia_pagination.py     # Hypermedia pagination implementation
└── 3-hypermedia_del_pagination.py  # Deletion-resilient hypermedia pagination implementation
```

## Data Source
The dataset used in this project is contained within a CSV file named `Popular_Baby_Names.csv`. This file includes information about popular baby names, such as year of birth, gender, ethnicity, name, count, and rank.

## Requirements
- Python 3.x
- `csv` module (included in standard library)
- `math` module (included in standard library)
- Basic knowledge of pagination and Python programming

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/harystyleseze/alx-backend.git
   ```
2. Navigate to the directory:
   ```bash
   cd alx-backend/0x00-pagination
   ```
3. Ensure that you have the `Popular_Baby_Names.csv` file in the same directory.

## Usage
You can run the implementations directly using Python. Each file contains a class `Server` that manages the pagination of the dataset.

### Example
To test the pagination functionalities, you can run the provided main scripts:

- For simple pagination:
  ```bash
  python3 1-main.py
  ```

- For hypermedia pagination:
  ```bash
  python3 2-main.py
  ```

- For deletion-resilient hypermedia pagination:
  ```bash
  python3 3-main.py
  ```

## Contributing
Contributions are welcome! If you would like to contribute to this project, please fork the repository and submit a pull request.

## License
This project is open-source and available under the MIT License. 

## Acknowledgments
- Thanks to the educational resources and community support that made this project possible.

