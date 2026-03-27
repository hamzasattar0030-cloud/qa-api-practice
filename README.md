# QA API Practice

This repository demonstrates practical quality assurance (QA) skills through API testing and structured bug reporting.

## Overview

This project showcases hands-on experience with:

* API testing using Postman
* Writing test cases and validation logic
* Creating structured bug reports (Jira-style)
* Executing both positive and negative test scenarios

## Features

* API endpoint testing using Postman
* Validation of response status codes and data
* Positive and negative test scenarios
* Structured test case documentation
* Jira-style bug reporting with clear reproduction steps

## Project Structure

* `jsonplaceholder_api_tests.postman_collection.json`
  Postman collection containing API requests and test scripts

* `postman_test_case.md`
  Documented API test cases including expected results and validation logic

* `jira_bug_report.md`
  Example bug report following a Jira-style structure

* `README.md`
  Project overview and documentation

## API Testing Details

Tested endpoints from:
https://jsonplaceholder.typicode.com/

### Example Tests

**Positive Test**

* Endpoint: `/posts/1`
* Expected: Status code 200 and valid response data

**Negative Test**

* Endpoint: `/posts/9999`
* Expected: Status code 404 or empty response `{}`

## Tools Used

* Postman (API testing)
* GitHub (version control and documentation)

## Skills Demonstrated

* API testing
* Test case design
* Bug reporting
* Response validation
* Positive and negative testing
* Analytical problem-solving

## How to Run

1. Download and install Postman
2. Import the collection file:

   * `jsonplaceholder_api_tests.postman_collection.json`
3. Run the requests inside the collection
4. View test results in Postman

## Author

Hamza Sattar
GitHub: https://github.com/hamzasattar0030-cloud
