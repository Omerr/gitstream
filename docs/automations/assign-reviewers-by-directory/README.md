# Assign Reviewers by Directory

Automatically assign code reviewers based on directory structure. Optionally, you can substitue `require-reviewers` for `add-reviewers` to make review from the specified teams and individuals mandatory.

![Assign Reviewers by Directory](assign_reviewers_by_directory.png)

Conditions (all must be true):

* The PR contains changes to JavaScript files inside the `src/ui` directory.

Automation Actions:

* Add a user named `my-teamate` and a team named `my-organization/ui-team` as reviewers. These should be customized to match your organization.
* Post a comment explaining why these reviewers were assigned.

!!! example "Assign Reviewers by Directory"
    ```yaml+jinja
    --8<-- "docs/downloads/automation-library/assign_reviewers_by_directory.cm"
    ```
    <div class="result" markdown>
      <span>
      [:octicons-download-24: Download this example as a CM file.](/downloads/automation-library/assign_reviewers_by_directory.cm){ .md-button }
      </span>
    </div>