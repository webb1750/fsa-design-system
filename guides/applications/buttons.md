---
layout: guide
parent: "Applications"
title: "Buttons"
intro: "FSA applications shall have the same look and feel, along with having a consistent naming convention for the most used buttons. Below you will find guidelines on how to use specific style related to various actions and features where a button is used."

---

## Variations and States

The below buttons are the default variations available for use in the FSA Design System. For further details on variations and states, refer to [Button Components]({{ site.baseurl }}components/buttons/).

<div class="dut-button-demo__section">
  <button class="fsa-btn fsa-btn--primary" type="button">Primary</button>
  <button class="fsa-btn fsa-btn--secondary" type="button">Secondary</button>
  <button class="fsa-btn fsa-btn--tertiary" type="button">Tertiary</button>
  <button class="fsa-btn fsa-btn--primary" disabled="disabled" type="button">Disabled</button>
  <button class="fsa-btn fsa-btn--flat" type="button">Cancel</button>
</div>

### Primary
A primary style shall be applied to a button that represents the top priority action a User might take in a given context. Submitting a form or continuing a stepped process would be considered primary.

### Secondary
A secondary style shall be applied to buttons that are not top priority, may be viewed as contrary to progress, or the action is relevant for adjacent features and functionality. An example of this would be a button that is labeled "View Producer" that displays data on the same screen without continuing a process.

### Tertiary
A tertiary style shall be applied only to buttons that perform a **destructive** action. A "Delete" button is a good example of an action that requires the tertiary style.

### Disabled
The disabled state shall be applied to any buttons unable to be clicked by a User, but should remain present and visible as an action that can be performed once other criteria is met.

### Flat
In most cases, a button labeled as "Cancel" should be shown with the Flat style which looks similar to a text link. By giving this button very low priority and prominence on the screen, it will not be easily mistaken as an action to take without contemplation from a User. Canceling a process can be destructive in nature, but it does not remove stored data from the database.

## General Guidelines:

 * All buttons shall use an action word to start the label. Eg. "View Details" vs. "Details"
 * A Cancel button shall not be used unless the online form uses a multi-step process
 * A Cancel button shall be used in a Multi-step or multiple screen process so the User feels safe that they are aborting a process
 * A Cancel or Close button action shall clear the contents of the online form for security/privacy purposes
 * When used, the Cancel button should appear as a link (i.e. `fsa-btn--flat` variation) or Secondary button
 * Buttons shall align to the left with primary or progressive/affirmative action on left, and secondary or regressive/dismissive action on right.

## Multi-Step Process Guidelines:

 * A **regressive** action shall be left-aligned, followed by right-aligned **progressive** action(s)
 * Back and Next can be used as button labels
 * The saving of data or state is implied and clicking the **"Regressive"** button shall not delete data that has been entered
 * Save or Submit can be used on the final step

## Reset and Clear Guidelines:

 * Reset is defined as removing all data and returning to the initial state of the application or online form inputs
 * Clear is defined as removing all data from application or online form fields
 * Reset and Clear buttons, if used, shall not be placed near a Primary button such as Next, Submit, or Save

## Which Label to Use?

<button class="fsa-btn fsa-btn--primary" type="button">Submit</button> vs. <button class="fsa-btn fsa-btn--primary" type="button">Save</button>

Use Submit for a button label when providing data that will not be stored, or if the data is submitted by an anonymous User. Use a Save label when the User is authenticated and will be updating data within a system.

 * Submit - Use for submitting data to generate a report
 * Save - Use for updating User profile information or preferences.

 ___

<button class="fsa-btn fsa-btn--primary" type="button">Search</button> vs. <button class="fsa-btn fsa-btn--primary" type="button">Submit</button>

Search shall be used as the button label when the application is performing a query and returning results. The Search label on a button is more ubiquitous on the web and Users are accustomed to looking for this functionality on a screen.

___

<button class="fsa-btn fsa-btn--primary" type="button">Back</button> vs. <button class="fsa-btn fsa-btn--flat" type="button">Cancel</button> vs. <button class="fsa-btn fsa-btn--primary" type="button">Exit</button>

When returning to a previous screen or step, use Back as the button label. When ceasing a process, such as updating your profile, use Cancel as the button label. Exit shall not be used in the context of returning to a previous screen, as it could imply exiting the application as opposed to the process in the application.

___

<button class="fsa-btn fsa-btn--primary" type="button">Refresh</button> vs. <button class="fsa-btn fsa-btn--primary" type="button">Reload</button> vs. <button class="fsa-btn fsa-btn--secondary" type="button">Reset</button>

When data or a state in the application has changed, it is recommended to use Refresh as a label. The Reload label implies getting more data, while Refresh is a more general and User friendly term. Reset implies clearing data and returning to the initial state of data.

___

<button class="fsa-btn fsa-btn--flat" type="button">Cancel</button> vs. <button class="fsa-btn fsa-btn--secondary" type="button">Cancel</button>

In general, all FSA applications should use the Flat style for a Cancel button. A Cancel button should utilize the secondary button style within a modal or popup window and the User needs to Cancel the action being performed.

___

<button class="fsa-btn fsa-btn--tertiary" type="button">Delete</button> vs. <button class="fsa-btn fsa-btn--secondary" type="button">Reset</button>

A button shall use the Tertiary style when the action taken has destructive capabilities. While Reset is an action that removes data from the screen, it should not be used to remove data from a database or other data storage.

___



## Common Button Labels and Functionality

<table class="fsa-table fsa-table--responsive">
    <thead>
        <tr>
            <th scope="col">Button Label</th>
            <th scope="col">Functionality</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Add</button>
                </p>
                <p>(Add [noun])</p>
            </td>
            <td>Add data, add new row, add new template for data entry</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Approve</button>
                </p>
            </td>
            <td>
                <p>Application specific button designed to be a single source of approval</p>
                <p>NOTE: Having an Approve button as compared to an Approve checkbox paired with a Submit button.</p>
            </td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Back</button>
                </p>
            </td>
            <td>Return to the previous page in the application.</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Calculate</button>
                </p>
                <p>(Calculate [noun])</p>
            </td>
            <td>Perform Calculation</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--flat" type="button">Cancel</button>
                </p>
                <p>(Cancel [noun])</p>
            </td>
            <td>
                <p>Stop current action and cancels out of the process.  Returns users to the page where the action was initiated.</p>
                <p>NOTE: If data has been entered, a confirmation message shall be displayed so the user can confirm they want to cancel.</p>
            </td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--secondary" type="button">Clear</button>
                </p>
            </td>
            <td>
                <p>Clears screen or form of all data.</p>
                <p>This button should be used with caution and generally only on pages where data is not actually saved, such as search pages or calculator type applications. When used, this button clears all fields on the page of all values.</p>
            </td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <a href="#" class="dut-button-demo__cancel-link">Close</a> [X]
                </p>
            </td>
            <td>Closes a child (popup or modal) window. A close text link paired with an "X" icon shall be used within a popup or modal window.</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Continue</button>
                </p>
            </td>
            <td>Go to the next page in a multi-step process.  This option is intended primarily for informational pages where no information is entered on the page.</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--tertiary" type="button">Delete</button>
                </p>
                <p>(Delete [noun])</p>
            </td>
            <td>
                <p>Allows the user to delete specific data or a record.</p>
                <p>NOTE: Shall require a confirmation question, such as a pop-up, with a Yes/No response for the user to confirm the deletion. Information about what is being deleted shall also be displayed for the user.</p>
            </td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Download</button>
                </p>
                <p>(Download [noun])</p>
            </td>
            <td>Download an application file to a user's storage device.</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Export</button>
                </p>
            </td>
            <td>Download data in various templated formats.</td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Filter</button>
                </p>
                <p>(Filter [noun])</p>
            </td>
            <td>
                <p>Remove all data from data set, except that which matches the selected criteria.</p>
                <p>NOTE: Rather than having a filter button, the Farm Programs team would like to explore various types of filtering. This button may still be necessary but Farm Programs would like to see other options.
                </p>
            </td>
        </tr>

        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Go to Application</button>
                </p>
            </td>
            <td>Allows users to access another application to view or update data.  Opens new application in a separate tab.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Log in</button>
                </p>
            </td>
            <td>Enter an application in an authenticated state.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Log out</button>
                </p>
            </td>
            <td>Exit an application currently in an authenticated state and return to Log in screen.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">No</button>
                </p>
            </td>
            <td>Decline response to an action to be taken, such as deleting data or a record.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Refresh</button>
                </p>
            </td>
            <td>Refreshes the data on the page. Primarily used after data has been updated in another application.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--secondary" type="button">Reset</button>
                </p>
            </td>
            <td>
                <p>Reset fields to the default field values(s) or previously saved value(s).</p>
                <p>NOTE: If data had been saved by the user that varies from the default value(s), the reset will refresh to the most recently saved value(s).</p>
            </td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Save</button>
                </p>
                <p>(Save [noun])</p>
            </td>
            <td>Save data and remains on the current page.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Save &amp; Continue</button>
                </p>
            </td>
            <td>Saves data on the current page of a multi-step or multi-screen process and continues to the next page.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Search</button>
                </p>
            </td>
            <td>Performs a query based on criteria submitted</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Select</button>
                </p>
            </td>
            <td>Initiate a Selected Action</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Submit</button>
                </p>
                <p>(Submit [noun])</p>
            </td>
            <td>
                <p>Send data to an application process, such as saving to a database. Returns users to the page where the action was initiated or to the home page.</p>
                <p>NOTE: Data is recorded on multiple pages in a multi-page process. Save or Save &amp; Continue would be the options through each of those pages. However on the page where the producer signature is recorded, the option would be to “Submit” because recording the producer signature signifies the application is being submitted to FSA for approval consideration. Status of the contract/application would then generally go from “initiated” to “filed” or “signed” as required by the applicable program application.
                </p>
            </td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Upload</button>
                </p>
                <p>Upload (Upload [noun])</p>
            </td>
            <td>Upload data file from a user’s storage device to the web application.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">View</button>
                </p>
                <p>(View [noun])</p>
            </td>
            <td>Show additional information or detailed information about item.</td>
        </tr>
        <tr>
            <td aria-label="Button Label" scope="row">
                <p>
                    <button class="fsa-btn fsa-btn--primary" type="button">Yes</button>
                </p>
            </td>
            <td>Confirmation response to an action to be taken, such as deleting data or a record.</td>
        </tr>

    </tbody>
</table>

## Related Resources

 * [Button Components]({{ site.baseurl }}components/buttons/)
