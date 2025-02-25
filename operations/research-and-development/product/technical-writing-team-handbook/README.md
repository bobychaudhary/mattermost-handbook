# Technical Writing Team Handbook

## Technical Writing Handbook

Mattermost Technical Writers focus primarily on writing, editing, structuring, and maintaining Mattermost technical and product documentation, end user documentation for Mattermost Channels, Boards, and Playbooks, as well as developer documentation and the company Handbook. Technical Writers also manage in-product microcopy, provide editorial reviews for all documentation across the organization, and work closely with the community to improve documentation.

### Areas of responsibility \(AORs\)

Documentation and technical writing at Mattermost covers \(but isn't limited to\) the following verticals:

* Channels
  * Mattermost Cloud
  * Self-managed deployments
  * Messaging features and functionality
* Playbooks
* Boards
* Growth
  * Customer Portal
  * Telemetry
* Apps Framework and Marketplace

Other areas of documentation include:

* Mattermost Handbook
* Integrations \(developer documentation, plugin documentation, and developer journey\)
* Documentation metrics:
  * Docs page ratings via Google Analytics
  * Google Analytics metrics for page visits, read times, and bounce rates
  * Customer feedback analysis
  * Metrics dashboards using RudderStack
* In-product messaging and interface
* GitLab documentation for:
  * [GitLab Mattermost docs](https://docs.gitlab.com/omnibus/gitlab-mattermost/%20)
  * GitLab helm chart docs
* Developer documentation for:
  * [developers.mattermost.com](https://developers.mattermost.com), including Contribute, Integrate, and Extend sections
  * [api.mattermost.com](https://api.mattermost.com)
  * General developer experience docs, e.g. code samples, best practices, and tutorials
* Community and doc review process
  * Process for Doc Up plugin
  * Docs review and release coordination
  * Community Help Wanted doc issues
* Content and processes
  * PR reviews across the organization
  * Documentation processes for release PRs

Please reach out to the [Documentation Working Group](https://community.mattermost.com/private-core/channels/dwg-documentation-working-group) for any questions.

### Contributing to documentation

The basic outline for getting started with contributions is provided in the [README](https://github.com/mattermost/docs/blob/master/README.md) of the docs repo. If you have write access to the repo, you can create a branch off master and work on that.

Once complete, submit your Pull Request \(PR\). Ensure that you assign appropriate approvers and labels - if you've forked the repo or don't have the correct repo permissions you may not be able to do this, so you can skip this step. Read more about the review process [here](https://developers.mattermost.com/contribute/getting-started/code-review) - it applies to various types of contributions including documentation.

## PR tips and best practices

* Try to submit files in batches rather than single PRs for each file update. This reduces the PR load and also groups your changes more effectively.
* When there are lots of changes requested, especially on a docs PR that doesn't require QA testing, you can use the "Add suggestion to batch" feature in GitHub to commit all of the suggestions at once. You need to be on the **Files changed** tab to use this feature, though it's also shown on the **Conversation** tab. By batching your suggestions, you can use one commit message such as "Added batch suggestions from @Carrie Warner". This just makes the commit history of the PR a lot more readable and useful for everyone reviewing it.
* Descriptive PR titles and commit messages go a long way, especially when the PR is referenced in the future. The default PR titles that GitHub gives us like "Updated README.md" are not very helpful because there's no way to know the purpose of the PR by reading the title. For example, if the whole file was translated to Japanese because we realize that's our main audience, that information isn't obvious unless you open the PR and read it - or if it's in the PR title.

### Submitting feature documentation

Feature documentation is a joint effort between Product Managers and Technical Writers. In the same way that we want to empower everyone to contribute to our documentation, Product Managers are encouraged to write MVP documentation for their product/feature. 

If your PR is for a new feature, major update to an existing feature, or a fix that impacts the current documentation, it's recommended that you include documentation around the change. This is helpful in providing context for reviewers, and also ensures the content can be added to the documentation quickly.

You can contribute documentation in one of the following ways:

* Update the relevant page on [docs.mattermost.com](https://docs.mattermost.com), and submit a PR for that. This PR is submitted to the docs repo, reviewed by the relevant team members, and merged from there.
* Submit your documentation as a new file, including the context and changes, any code samples, and processes. You can submit this as part of your PR, or you can open a new PR in the docs repo and include a link to your open code PR.

We don't expect a huge body of documentation or that it's perfectly-written - but rather a clear, concise outline of the change which can be added to our documentation. The content can be provided as a list, rough notes, or you can use the example below for content and structural guidance if your documentation is quite detailed.

**Note:** Due to the cadence of the release cycle, feature documentation needs to be complete and submitted as [per the release process](https://handbook.mattermost.com/operations/research-and-development/product/release-process/feature-release#e-t-minus-15-working-days-judgment-day) to allow sufficient time for review and to ensure it's included in the release documentation update.

The supplied content can be provided informally, in bullet points, or rough notes in a Google Doc/Jira issue/on the PR itself. Refinements are made collaboratively.

**Feature documentation MVP \(PMs\)**

This is a guideline of what MVP feature documentation can include. Requirements vary based on the scope of the change, so not everything will always be needed:

* A link to the feature/product's tech spec.
* Links to any relevant Jira/GitHub issues.
* A description of the product/feature/update which forms the basis of the documentation.
* Steps for any processes or procedures \(configuration of a feature, troubleshooting, etc\).
* Any FAQs or troubleshooting questions if relevant.
* Any limitations, issues, or known problems.
* Configuration settings and examples for the `config.json` file if relevant.
* \(If possible\) Suggestions of where in the docs the content should go.

When the content has been refined and approved in draft format:

* The Product Manager/Technical Writer creates a branch off the relevant documentation release branch.
* The documentation is updated with the approved content in that branch.
  * If there are multiple pages to update for a specific feature/change please keep them all in the same branch for ease of management.
* The PR is submitted and relevant reviewers added, including an editor \(not the Technical Writer who wrote the docs\), for final review.
  * Include the link to the server/webapp repo issue in your PR for reference purposes.
* Once all reviews are complete, the PR is marked as **Reviews Complete** and merged into the documentation release branch by @amyblais.

You can read more about the review process [here](https://developers.mattermost.com/contribute/getting-started/code-review).

You can find additional guidance around formatting [here](https://handbook.mattermost.com/operations/operations/company-processes/publishing/publishing-guidelines/voice-tone-and-writing-style-guidelines/documentation-style-guide#using-restructuredtext-markup-rst).

Once your PR is submitted, there's a review process that includes an editorial review, a PM review, and sometimes a dev review. During the editorial review, editors may make punctuation and/or terminology changes and commit them to save time on the review process. This only applies to punctuation/terminology - content suggestions and questions will follow the usual review and discussion process.

Once the review is complete, we'll move your contribution to the appropriate part of [docs.mattermost.com](https://docs.mattermost.com) \(if it's not there already\) and then merge it. We'll share the URL and you can edit it at any time if you need to.

### Submitting documentation with your PR

We want to empower everyone to contribute to our documentation, and be comfortable submitting documentation for contributions. As such, we don't expect every contribution to adhere to our style guide when first submitted.

During the review process the editorial team also provides feedback on style elements to bring the submission in line with the [Documentation Style Guide](https://docs.mattermost.com/guides/core.html#documentation-style-guide).

Here are some guidelines:

* When submitting a code PR, please include updated documentation if applicable.
* The documentation update can be in the form of a bullet list or an outline.
* Label the PR as **Docs Needed**/**Editor Review** and tag @justinegeffen or @carriewarnermm.
* The documentation you've submitted will be reviewed.
* At times, the editors may make and commit stylistic changes \(such as punctuation\) but any content changes will be added as a suggestion for the submitter's consideration.
* Once the PR is approved, it will be merged, and the documentation will be updated.

You can read more about the review process [here](https://developers.mattermost.com/contribute/getting-started/code-review).

**Note:** This process does not apply to the [API Documentation requirements](https://github.com/mattermost/mattermost-api-reference) as it is updated automatically and isn't part of the documentation process.

### Adding reviewers to PRs

Mattermost documentation covers a number of different topics. For documentation, the following reviewers are recommended:

**Editor Review**

* Carrie Warner \(@cwarnermm\)
* Justine Geffen \(@justinegeffen\)

**Product Manager Review**

* Channels: Katie Wiersgalla \(@wiersgallak\)
* Security: Katie Wiersgalla \(@wiersgallak\)
* Cloud: Katie Wiersgalla \(@wiersgallak\)
* Playbooks: Ian Tao \(@tao\)
* Boards: Winson Wu \@winsonwu\)
* Licensing: Jason Blais\(\@jasonblais\)
* Mobile and desktop app: Eric Sethna \(@esethna\)
* Apps and Marketplace: Aaron Rothschild \(@aaronrothschild\)
* Handbook and Process; Community: Jason Blais \(@jasonblais\)

**Dev Review**

If your change requires dev review add the developer/s you've been working with as the reviewer/s. If you're unsure who to add as a dev reviewer you can select one of the team leads below:

* Boards: Scott Bishel \(@sbishel\)
* Integrations: Catalin Tomei \(@catalintomai\)
* Playbooks: Jesse Hallam \(@lieut-data\)
* Channels: Martin Kraft \(@mkraft\)
* Growth: Maria Nuñez \(@marianunez\)
* SRE: Joram Wilander \(@jwilander\) \(\interm\)
* Cloud Platform: Joram Wilander \(@jwilander\)
* Mobile: Elias Nahum \(@enahum\)
* Web App and Desktop App: Dean Whillier \(@deanwhillier\)
* Server/infra: Joram Wilander \(@jwilander\)
* Cloud: Joram Wilander \(@jwilander\)
* Security: Daniel Schalla \(@dschalla\)
* QA: Saturnino Abril \(@saturninoabril\)
* Handbook and Process: Jason Blais \(@jasonblais\)

The full list of R&D teams is available [here](https://docs.google.com/spreadsheets/d/1lH8QIjQGEoGospDUdVs_LQ_i2b82I1ce6W7z18vhPTQ/edit#gid=0).

### Requesting Documentation via Doc Up

Requests for documentation can be made within [community.mattermost.com](https://community.mattermost.com), using the Doc Up plugin embedded in the post menu.

![Access the Doc Up plugin by hovering over a message and clicking the &quot;...&quot; menu.](../../../.gitbook/assets/doc-up-plugin.png)

When you select Doc Up and choose **Admin** as the issue type, an issue is generated in the GitHub docs repo, and added to the issues list. An update is listed in the Documentation channel, with the issue link.

You can also select **Developer** or **Company Handbook** to direct the Doc Up request to the appropriate repo.

As the issues are open to the community, the more information provided in the issue the better.

Review the issue in the [docs repo](https://github.com/mattermost/docs/issues?q=is%3Aopen+is%3Aissue), [developer documentation repo](https://github.com/mattermost/mattermost-developer-documentation/issues?q=is%3Aopen+is%3Aissue), or [handbook repo](https://github.com/mattermost/mattermost-handbook/issues?q=is%3Aopen+is%3Aissue) and add any links to appropriate documentation and/or Jira tickets. This ensures that the assignee is able to take on and complete the work within the turnaround times.

**Turnaround time**

When the issue has been created, please follow these guidelines to assign [labels](https://developers.mattermost.com/contribute/getting-started/labels). This ensures that the issues are prioritized appropriately.

There are a number of variables at play, such as review process, current workload, and type of work required which makes it difficult to provide a hard and fast time-frame for completion. Large projects might be moved to Jira if required.

**Assignees**

Documentation does not have to be written by the Technical Writer/s. You can raise an issue, complete the requirement, and submit a Pull Request.

**Community involvement**

We really want the community to own the docs as much as possible. In light of this, please mark your issue as **Help Wanted** so that community members are able to identify work that they’re able to assist with. If your documentation request/issue applies to a repository other than _mattermost/docs_, you can use the **Docs Needed** and **Editor Review** labels and/or ping @justinegeffen or @cwarnermm.

### i18n contributions

**Note: This process is in flight.\***

Our product documentation is available for translation contributions. Join the [i18n channel](https://community.mattermost.com/core/channels/localization) on our Community server and connect with our translation community members. The documentation translation process is still being defined.

Currently, submitting a translation PR follows the same writing and editing process as other PRs. However, there are additional considerations to bear in mind when submitting your PR as these assist with the approval and merge process:

1. Do you have an active test instance running with the integrations guide translated so we can validate the rendering and formatting?
2. If the content you're translating includes screenshots should we keep the original English versions of the screenshots, or consider translated versions of them too?
3. If the intention is to translate the screenshots, is there a proposed process for keeping them up to date?
4. Have at least one member of UX team and one member of Apps PM team review the user experience in choosing different languages.
5. To maintain high standards for translated documentation, set up a process to notify translators when something is changed in the English-version of the docs, and expectation on correcting translations for new releases.
6. Decide if we want to indicate translations level - e.g. “Alpha” or “Beta” for translations that are in progress.
7. Test you can successfully rate a translated docs page by selecting a rating emoji. Ping @justine.geffen for validation of this.

## General contribution workflow

### DWG board

If you have a feature, UI copy, or general documentation requirement, please create a card on the [DWG incoming requests board](https://community.mattermost.com/plugins/focalboard/workspace/g4k9s1f953n4bytz5f9sz9orer/shared/bm47zpk19p3b4ufb3krjt4usgfo/vwgh41ounkbr4d8n3xsbjggoy9y?r=k4z1qsm4y5tntiyqt78fcbksmhh).

For best results, include as much content, context, and detail as possible. Once you're done, tag @carrie.warner or @justine.geffen. The board is checked daily and cards are prioritized based on current workload.

If the card is for documentation related to a release, the documentation needs to be complete at least 10 days prior to release. Please ensure you allow sufficient time for your request to be completed or it will be moved to the next available slot.

### Editing requests

When submitting a PR for documentation, whether it's a minor update, a new piece of content, or a content proposal, please add the **Editor Review** label \(if possible\). Once the Technical Writer/Editor has reviewed the PR they'll remove the label. When all the requested reviews are complete, the **Reviews Complete** label is applied and the changes are merged.

### Providing editorial feedback

If you're asked to provide editorial feedback on a PR, and it's your first editorial feedback request, first read up on the review process [here](https://developers.mattermost.com/contribute/getting-started/code-review) to get an idea of what's expected in terms of turnaround time, type of feedback, and so on.

Editorial feedback is based on the guidelines laid out in the [Documentation Style Guide](https://docs.mattermost.com/guides/core.html#documentation-style-guide) as well as the [Voice, Tone, and Writing Style Guide](https://handbook.mattermost.com/operations/operations/publishing/publishing-guidelines/voice-tone-and-writing-style-guidelines).

### Formatting and Style Guide

The [Documentation Style Guide](https://docs.mattermost.com/guides/core.html#documentation-style-guide) and [UI text guidelines](https://docs.mattermost.com/process/documentation-UItext-guidelines.html).

## Community documentation involvement

Every month the Mattermost community plans, builds, tests, documents, releases, and supports new product improvements for Team Edition to benefit the user community. The Mattermost Enterprise Team does the same for Enterprise Edition to benefit the subscriber community.

A critical part of this development is documentation which ranges from feature documentation to FAQs, guides, and tutorials.

### Feature documentation

Feature documentation is a collaborative effort between the Product Manager and Technical Writer within a specific timeframe aligned with releases. Community members are welcome to assist, if the time expectations are manageable.

Feature request documentation is usually located in the [mattermost-server](https://github.com/mattermost/mattermost-server/issues?q=is%3Aopen+is%3Aissue+label%3ADocs%2FNeeded) repo and the [mattermost-webapp](https://github.com/mattermost/mattermost-webapp/pulls?q=is%3Aopen+is%3Apr+label%3ADocs%2FNeeded) repo and are labelled as `Docs/Needed`. As these are tied to a release \(and a deadline\) it’s best to only take on the work if you’re sure you can complete it on time. It’s understood that community members contribute in their available time, which is why this type of documentation isn’t usually the best option to take on.

### Help Wanted tickets/doc issues

Help Wanted tickets are generally not linked to a release and are more flexible in terms of timeline and delivery date. You can find the documentation Help Wanted tickets [here](https://github.com/mattermost/docs/labels/Help%20Wanted). To start working on one, assign it to yourself, add a comment indicating you’ll be working on it, find the relevant document in the [source](https://github.com/mattermost/docs/tree/master/source) directory, read through the [README](https://github.com/mattermost/docs/blob/master/README.md) file if you're not familiar with the process, and get started.

If you have any questions, you can post them in the [Documentation](https://community.mattermost.com/core/channels/documentation) channel and we'll be happy to help.

### Engineering/developer documentation

Most, if not all, contributions to the Mattermost project have a documentation impact. As part of the development and submission process, it’s recommended that the relevant documentation be updated \(or created\) and included in the PR. This provides consistency and accuracy in communicating the changes/new feature and cuts down on having multiple issues and PRs for related documentation.

Visit the [Contribute to Documentation](https://handbook.mattermost.com/operations/operations/publishing/publishing-guidelines/voice-tone-and-writing-style-guidelines/submitting-documentation-with-your-pr) page to get started with submitting documentation with your PR. You can read more about the review process [here](https://developers.mattermost.com/contribute/getting-started/code-review).

## GitHub training

GitHub training videos coming soon!
