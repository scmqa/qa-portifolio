Cypress Form Submission Test

Overview

This project demonstrates an automated test using Cypress to validate form submission functionality.

The test simulates user interaction by entering data into a form and verifying that the system responds correctly.

Technologies Used

- Cypress
- JavaScript

Test Scenario

The test validates whether a user can successfully fill out and submit a form.

Test Steps

1. Open the test page
2. Enter a valid email address
3. Submit the form

Expected Result

The system should display a success message confirming the form submission.

Actual Result

The form was successfully submitted, and the message "Your form has been submitted!" was displayed.

Test Status

Passed

Automation Code

describe('Form Test', () => {
  it('should fill form and submit', () => {
    cy.visit('https://example.cypress.io/commands/actions')

    cy.get('.action-email').type('test@email.com')
    cy.get('.action-form').submit()

    cy.contains('Your form has been submitted!').should('be.visible')
  })
})

Conclusion

The test confirms that the form submission functionality is working as expected.
