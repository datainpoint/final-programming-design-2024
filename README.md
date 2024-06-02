# final-programming-design-2024
Final: Programming Design 2024.

## 01. Define a function `factorial()` which returns the result of $n!$.

Source: <https://en.wikipedia.org/wiki/Factorial>

```python
def factorial(n: int) -> int:
    """
    >>> factorial(0)
    1
    >>> factorial(1)
    1
    >>> factorial(2)
    2
    >>> factorial(3)
    6
    >>> factorial(4)
    24
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `get_optimal_change()` in New Taiwan Dollar currency system. By saying "optimal" means the cashier has enough amount of all currency amounts in coins and notes, and the cashier strives for giving customer as few as possible.

```python
def get_optimal_change(sale_price: int, paid: int) -> dict:
    """
    >>> get_optimal_change(35, 50)
    {500: 0, 100: 0, 50: 0, 10: 1, 5: 1, 1: 0}
    >>> get_optimal_change(69, 100)
    {500: 0, 100: 0, 50: 0, 10: 3, 5: 0, 1: 1}
    >>> get_optimal_change(124, 150)
    {500: 0, 100: 0, 50: 0, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 200)
    {500: 0, 100: 0, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 500)
    {500: 0, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 1000)
    {500: 1, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(1124, 1500)
    {500: 0, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(1124, 2000)
    {500: 1, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a class `Prime` which instantiates objects with 2 methods `get_nth_int()` and `get_sequence()`.

Source: <https://en.wikipedia.org/wiki/Prime_number>

```python
class Prime:
    """
    >>> prime = Prime(5)
    >>> prime.get_nth_int(1)
    2
    >>> prime.get_nth_int(2)
    3
    >>> prime.get_nth_int(3)
    5
    >>> prime.get_nth_int(4)
    7
    >>> prime.get_nth_int(5)
    11
    >>> prime.get_sequence()
    [2, 3, 5, 7, 11]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a class `Rot13` which instantiates objects with 2 methods `rotate_character()` and `rotate_sentence()`.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
class Rot13:
    """
    >>> rot13 = Rot13()
    >>> rot13.rotate_character("A")
    'N'
    >>> rot13.rotate_character("B")
    'O'
    >>> rot13.rotate_character("L")
    'Y'
    >>> rot13.rotate_character("M")
    'Z'
    >>> rot13.rotate_character("a")
    'n'
    >>> rot13.rotate_character("b")
    'o'
    >>> rot13.rotate_character("l")
    'y'
    >>> rot13.rotate_character("m")
    'z'
    >>> rot13.rotate_sentence("Abj vf orggre guna arire.")
    'Now is better than never.'
    >>> rot13.rotate_sentence("Now is better than never.")
    'Abj vf orggre guna arire.'
    >>> rot13.rotate_sentence("Rkcyvpvg vf orggre guna vzcyvpvg.")
    'Explicit is better than implicit.'
    >>> rot13.rotate_sentence("Explicit is better than implicit.")
    'Rkcyvpvg vf orggre guna vzcyvpvg.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `import_mlb_teams_json()` which imports `mlb_teams.json` in working directory.

```python
def import_mlb_teams_json() -> list:
    """
    >>> mlb_teams = import_mlb_teams_json()
    >>> type(mlb_teams)
    list
    >>> len(mlb_teams)
    30
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a function `find_teams_ballpark()` which returns the ballpark given team name and `mlb_teams.json` in working directory.

```python
def find_teams_ballpark(team: str) -> str:
    """
    >>> find_teams_ballpark("Boston Red Sox")
    'Fenway Park'
    >>> find_teams_ballpark("New York Yankees")
    'Yankee Stadium'
    >>> find_teams_ballpark("Los Angeles Dodgers")
    'Dodger Stadium'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `find_ballpark_full_address()` which returns the ballpark's full address in the format of `address, city, state, country` separated by comma given team name and `mlb_teams.json` in working directory.

```python
def find_ballpark_full_address(team: str) -> str:
    """
    >>> find_ballpark_full_address("Boston Red Sox")
    '4 Jersey Street, Boston, MA, United States'
    >>> find_ballpark_full_address("New York Yankees")
    'One East 161st Street, Bronx, NY, United States'
    >>> find_ballpark_full_address("Los Angeles Dodgers")
    '1000 Vin Scully Avenue, Los Angeles, CA, United States'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `import_movies_release_info()` which imports `movies.csv` and `release_info.csv` as Pandas DataFrames in working directory.

```python
def import_movies_release_info() -> tuple:
    """
    >>> movies, release_info = import_movies_release_info()
    >>> type(movie)
    pandas.core.frame.DataFrame
    >>> type(release_info)
    pandas.core.frame.DataFrame
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `find_the_shawshank_redemption_release_info()` which returns the release information of the movie "The Shawshank Redemption".

```
                       title        country release_date
0   The Shawshank Redemption         Canada   1994-09-10
1   The Shawshank Redemption  United States   1994-09-13
2   The Shawshank Redemption  United States   1994-09-22
3   The Shawshank Redemption         Canada   1994-09-23
4   The Shawshank Redemption         Mexico   1994-09-23
..                       ...            ...          ...
63  The Shawshank Redemption          Egypt   2021-04-18
64  The Shawshank Redemption         Israel   2021-09-14
65  The Shawshank Redemption     Kazakhstan   2022-06-04
66  The Shawshank Redemption          China   2023-04-20
67  The Shawshank Redemption    South Korea   2024-05-08

[68 rows x 3 columns]
```

```python
def find_the_shawshank_redemption_release_info() -> pd.core.frame.DataFrame:
    """
    >>> the_shawshank_redemption_release_info = find_the_shawshank_redemption_release_info()
    >>> the_shawshank_redemption_release_info.shape
    (68, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `find_the_shawshank_redemption_release_info_in_taiwan()` which returns the release information of the movie "The Shawshank Redemption" in Taiwan.

```python
def find_the_shawshank_redemption_release_info_in_taiwan(nth_release: str) -> str:
    """
    >>> find_the_shawshank_redemption_release_info_in_taiwan("1st") # First release
    "1995-03-10"
    >>> find_the_shawshank_redemption_release_info_in_taiwan("2nd") # Re-release
    "2020-03-13"
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```