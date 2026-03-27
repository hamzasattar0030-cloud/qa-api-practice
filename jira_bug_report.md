# Jira-Style Bug Report

## Issue Type
Bug

## Summary
Registration form accepts invalid characters in name field

## Description
The registration form allows users to enter numbers and special characters into the name field without validation. This may result in invalid user data being submitted.

## Steps to Reproduce
1. Open the registration page
2. Enter `Hamza123!!!` in the name field
3. Complete the remaining mandatory fields
4. Submit the form

## Expected Result
The system should reject invalid characters and only allow alphabetical input in the name field.

## Actual Result
The system accepts numbers and special characters in the name field and allows form submission.

## Priority
Medium

## Severity
Medium

## Environment
Web application - desktop browser

## Attachments
Optional screenshot if available
