# second_trial_count_words_poblano
Implementing package creation and continuous integration workflow

1. Create a repo (as we do it usually)
2. Create a virtual environment `python3 -m venv venv`
3. We borrow the files from our previous repo
    - `count_words.py`
    - `test_words.py`
4. **Make the package pip-installable**
   - We need a file called `setup.py`
   - Before we create the file, we need to have our module in the package folder.
   - We create a folder called `count_words_package`
   - We also need a folder for the tests called `tests`
   - All test*py files go to tests folder
   - the counts_words.py file go to count_words_package
   - We need to create an empty `__init__.py` files in both folders
   - We then have to modify our test*py files so that we can still access the count_words.py
     `from count_words_package.count_words import WordCounter`
   - Implement the setup.py
     - create it first `touch setup.py`
     - You just need to copy the file in the online notes and make changes accordingly
   - Make sure to create the `requirements.txt` file by `pip freeze > requirements.txt`
   - Finally type `pip install .`
   
	
