# Running the Tests

## Installing pytest
We recommend you install pytest and pytest-cache. pytest is a testing tool that will give you more flexibility over running your unit tests.

## To install pytest, run the following command:

pip3 install pytest pytest-cache
If you get a command not found response from your system, you can find a tutorial on how to install pip here.

If you want to check what the default version of pytest being used is, run the following:

pytest --version
If you choose not to install pytest, you can still run tests individually and skip the rest of this tutorial:

cd exercism/python/bob
python bob_test.py
## Running the Tests
## Run All Tests
To run all tests for a specific exercise (we will take the bob.py exercise as an example here), place yourself in the directory where that exercise has been fetched and run:

pytest bob_test.py
Note: To run the tests you need to pass the name of the testsuite file to pytest (generally, the file ending with _test.py), NOT the file you created to solve the problem (which is your implementation). This is because in the latter case, since there are no defined test cases in your implementation, pytest will just return a positive result, specifying that it ran zero tests. Like this:

=============================  bob.py  ==============================

---------------------------------------------------------------------

Ran 0 tests in 0.000s

OK
