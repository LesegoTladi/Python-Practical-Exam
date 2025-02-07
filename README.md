# Python-Practical-Exam

This repository contains the solutions for a Python practical exam. The exam consists of six independent questions focused on topics such as numerical computations, string manipulations, list operations, and working with pandas DataFrames.

## Overview

The exam requires you to implement various functions to solve specific problems. The questions are divided into three sections:

- **Section 1: Numerical Computation**
  - Functions for mathematical operations on numbers and matrices.
  
- **Section 2: Strings and Lists**
  - String manipulations and list operations.
  
- **Section 3: Dataframes**
  - Operations on pandas DataFrames to extract specific information.

## Requirements

Ensure you have the following Python libraries installed to execute the notebook:

- **numpy**
- **pandas**

You can install them using pip:

```bash
pip install numpy pandas
```

## Instructions

1. **Do not modify the structure of the notebook:**
   - **Do not add or remove cells** from the notebook.
   - **Do not change the names** of the required functions for testing.

2. **Independence of Questions:**
   - Each question is independent, and you can solve them in any order.
   - Avoid reusing functions between questions, as each one is designed to be solved individually.

3. **Code Submission:**
   - Ensure your code does not contain **syntax errors** or **indentation errors**.
   - If errors are encountered during testing, an error message will be provided. Use it to fix your code and resubmit.
   - You can submit your code **multiple times** to check for correctness before final submission.

4. **Function Implementation:**
   - Your code should only be placed inside sections marked with `# Your code here` comments.
   - Some expected outputs are provided to guide you in checking whether your implementation is correct.

## Questions

### Section 1: Numerical Computation

1. **Largest Square from a Rope**
   - Write a function `largest_square(x)` that computes the largest square area that can be formed from a rope of length `x`. The side length of the square must be an integer.

2. **Sum of Diagonals in a Square Matrix**
   - Write a function `sum_of_diagonals(matrix)` that computes the sum of the two diagonals of a square matrix. Ensure that if the dimension is odd, the center element is not counted twice.

### Section 2: Strings and Lists

3. **Vowel to Consonant Ratio**
   - Write a function `vowel_consonant_ratio(sentence)` that computes the ratio of vowels to consonants in a sentence, excluding punctuation marks and white spaces. The ratio should be rounded to two decimal places.

4. **Redact Every Third Word**
   - Write a function `redact_words(sentence)` that redacts every third word in a sentence using `#` symbols. Ensure that punctuation marks are not redacted.

5. **Separate Alphanumeric List into Three Categories**
   - Write a function `create_dictionary(character_list)` that separates a list containing alphanumeric characters into three lists: lowercase letters, uppercase letters, and numbers, sorted in ascending order.

### Section 3: Dataframes

6. **List Countries by Region and Income Group**
   - Write a function `find_countries_by_region_and_income(region, income_group)` that returns a list of countries for a specified region and income group, based on the provided dataframes.

## Example Output

The repository contains test cases for each function. Below are some example outputs:

```python
largest_square(12) == 9
largest_square(41.5) == 100
largest_square(324) == 6561

sum_of_diagonals(matrix) == 31
sum_of_diagonals(matrix) == 33

vowel_consonant_ratio("This is a random sentence!") == 0.62
vowel_consonant_ratio("Thomas! Where have you been?") == 0.83

redact_words("My dear Explorer, do you understand the nature of the given question?") == 'My dear ########, do you ########## the nature ## the given ########?'

create_dictionary([2,'j','K','o',6,'x',5,'A',3.2]) == {'numbers': [2, 3.2, 5, 6], 'uppercase': ['A', 'K'], 'lowercase': ['j', 'o', 'x']}

find_countries_by_region_and_income('South Asia','High income') == None
find_countries_by_region_and_income('Europe & Central Asia','Low income') == ['Tajikistan']
find_countries_by_region_and_income('Sub-Saharan Africa','Upper middle income') == ['Botswana', 'Gabon', 'Equatorial Guinea', 'Mauritius', 'Namibia', 'South Africa']
```

## Additional Notes

- **DataFrames:** The DataFrames (`country_map_df`, `population_df`, and `meta_df`) used in Section 3 are provided in the repository. Do not modify these DataFrames as this can lead to a negative mark.
- **Testing:** The notebook is designed to be executed in a Jupyter Notebook environment. Make sure to test your functions to confirm they work as expected before submission.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
