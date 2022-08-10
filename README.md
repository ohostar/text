# How to rub Robot framework tests

### Python installation

[Robot Framework](https://robotframework.org/) is implemented using [Python](http://python.org/), and a precondition to install it is having Python or its alternative implementation [PyPy](https://pypy.org/) installed. Another recommended precondition is having the [pip](https://pip.pypa.io/) package manager available.

Robot Framework requires Python 3.6 or newer.

### Installing Robot Framework

#### Installing using pip

> ```
> pip install robotframework
> ```

Verifying installation

> ```
> $ robot --version
> Robot Framework 5.0.1 (Python 3.10.6 on win32)
> ```

Selenium Library installation

> ```
> pip install --upgrade robotframework-seleniumlibrary
> ```

### Chrome webdriver installation

Download the latest Chrome webdriver from official site [https://chromedriver.chromium.org/downloads](https://chromedriver.chromium.org/downloads)

Make sure the driver version matches the installed version of Chrome

Include the ChromeDriver location in your PATH environment variable.

### VS Code extension

For syntax highlighting, auto-completion, etc. install this extension: **Robot Framework Language Server**

### Run Robot tests

To run all existing test just run the command below in the directory with tests. This command will run all files with **.robot** extension and create result report in the directory where command will used.

> ```
>  ~\Test.RobotFramework\tests $ robot .
> ```

Run test cases by Tags (e.g Smoke)

> ```
> robot -i Smoke .
> ```

Exclude test  cases by Tags

> ```
> robot -e Smoke .
> ```
