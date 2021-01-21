#11.1 warming up
Linting involves static analysis of source code, it includes checking for syntax errors and unused resources, missing includes and code formatting. Many IDEs include these sorts of checking but it is also important to be able to run these checks as part of CI process. For Python there are solutions that take care of some specific area of code checking and then there are tools that combine many linters like Flake8 or Pylama. I would choose either of these and possibly enforce generally used style guide for writing Python like PEP8.

Tesing should also be part of CI pipeline. The most common testing library for Python seems to be pytest. Python also has build-in testing framework: unittest. Robot and Cucumber can also be used with Python for acceptance testing.

Python is interpreted language so it is not always necessary to build it before execution. Depending on usecase it might however be needed. To build packages there are tools like PEX, pyInstaller. Software can also be packaged to be consumed through package managers like pip and Anaconda.

Popular alternatives to Jenkins and Github Actions include CI Circle and Travis. These both offer cloud based service. At this point I would take the cloud-based alternative as the release is going to happen soon and it might be too heavy to setup self-hosted solution at this time. Also as we are a small team and if we do not have any special requirements for the solutions there does not seem to be reasons to configure and mainain own solution.

