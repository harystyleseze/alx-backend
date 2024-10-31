# Caching Project

## Author
- **Name**: Harrison Eze
- **GitHub Username**: [harystyleseze](https://github.com/harystyleseze)

## Repository
- **GitHub Repository**: [alx-backend](https://github.com/harystyleseze/alx-backend)
- **Directory**: 0x01-caching

## Project Overview
This project implements various caching algorithms in Python. The caching system is designed to manage data in memory efficiently, ensuring quick access while optimizing memory usage. It includes several caching strategies, each demonstrating different approaches to managing stored data.

## Caching Algorithms Implemented
1. **FIFO (First In, First Out) Cache**
   - Discards the oldest data when the cache limit is reached.

2. **LIFO (Last In, First Out) Cache**
   - Discards the most recently added data when the cache limit is reached.

3. **LRU (Least Recently Used) Cache**
   - Discards the least recently accessed data when the cache limit is reached.

4. **MRU (Most Recently Used) Cache**
   - Discards the most recently accessed data when the cache limit is reached.

5. **LFU (Least Frequently Used) Cache**
   - Discards the least frequently accessed data, with a fallback to LRU if there's a tie.

## Installation
To use the caching algorithms, clone the repository and navigate to the project directory:

```bash
git clone https://github.com/harystyleseze/alx-backend.git
cd alx-backend/0x01-caching
```

## Usage
You can test each caching algorithm using the provided `main.py` files. Each file contains example usage demonstrating how to put and get items from the cache.

### Example
To run the FIFO cache example:

```bash
python3 2-main.py
```

## Testing
Make sure to have Python 3 installed. The algorithms can be tested by running the respective main files for each cache type.

## Contributing
Contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Special thanks to [ALX Africa](https://www.alxafrica.com) for providing the framework and learning resources for this project.
