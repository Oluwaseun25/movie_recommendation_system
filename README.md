

# Movie Recommendation System

## Project Overview

This project involves building a robust movie recommendation system using a hybrid approach, combining collaborative filtering and content-based methods to provide more accurate recommendations. The MovieLens dataset, along with data from IMDB, will be used to develop and test the system. This project will also explore big data technologies and cloud computing using AWS and Azure.

## Dataset

### MovieLens Dataset

The MovieLens dataset used in this project is from [GroupLens](http://movielens.org) and includes:

- **Ratings Data**: 32,000,204 ratings and 2,000,072 tag applications across 87,585 movies.
- **Time Span**: Data created by 200,948 users between January 09, 1995 and October 12, 2023.
- **Files**: 
  - `links.csv`
  - `movies.csv`
  - `ratings.csv`
  - `tags.csv`

#### File Structures

- **`ratings.csv`**: Contains ratings with columns `userId`, `movieId`, `rating`, `timestamp`.
- **`tags.csv`**: Contains tags with columns `userId`, `movieId`, `tag`, `timestamp`.
- **`movies.csv`**: Contains movie information with columns `movieId`, `title`, `genres`.
- **`links.csv`**: Contains identifiers with columns `movieId`, `imdbId`, `tmdbId`.

#### Usage License

- **Attribution**: Acknowledge the use of the dataset in publications.
- **Redistribution**: Can redistribute the dataset under the same license conditions.
- **Commercial Use**: Requires permission for commercial use.
- **Warranty**: Dataset is provided "as is" without any warranty.

For more details, see the original [README.md](data/README.md) file provided with the dataset.

#### Citation

To cite this dataset, use the following paper:

> F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4: 19:1–19:19. <https://doi.org/10.1145/2827872>

## Technologies

### Big Data Technologies

- **Apache Spark**: For distributed data processing.
- **Hadoop**: For storing and processing large datasets.

### Cloud Computing

- **AWS**: Utilize AWS services for scalable data processing and storage.
- **Azure**: Explore Azure for cloud-based machine learning and data analytics.

## Data Processing

To manage and process the large dataset files:

1. **Loading Data**: Use Pandas in Python to load and inspect data.
2. **Handling Large Files**: Read files in chunks if necessary.
3. **Cleaning Data**: Handle missing values and normalize data.

Example code to load data:

```python
import pandas as pd

# Load dataset files
movies = pd.read_csv('data/movies.csv')
ratings = pd.read_csv('data/ratings.csv')
tags = pd.read_csv('data/tags.csv')
links = pd.read_csv('data/links.csv')

# Inspect data
print(movies.head())
print(ratings.head())
print(tags.head())
print(links.head())
```

## Project Structure

- **`src/`**: Source code for the recommendation system.
- **`data/`**: Dataset files and scripts for data processing.
- **`notebooks/`**: Jupyter notebooks for exploratory data analysis.
- **`docs/`**: Documentation and reports.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Project**:
   - Execute the data processing scripts in the `src/` directory.
   - Train and evaluate the recommendation model.

4. **Verify Data**: Ensure dataset integrity by checking MD5 checksums.

```bash
md5sum *; cat checksums.txt
```

## Contributing

Feel free to contribute to the project by submitting issues or pull requests. For any questions, please contact [samuelawe842@gmail.com](mailto:samuelawe842@gmail.com).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- GroupLens Research for providing the MovieLens dataset.
- [MovieLens](http://movielens.org) for the recommendation service.
- [IMDB](http://www.imdb.com) for additional movie data.

For further information, visit the [GroupLens](http://grouplens.org) website.
```
