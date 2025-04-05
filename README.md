<div align="center">

<div align="center">


<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://www.khulnasoft.com/wp-content/uploads/2025/02/PR-Insight-Purple-2.png">
  <source media="(prefers-color-scheme: light)" srcset="https://www.khulnasoft.com/wp-content/uploads/2025/02/PR-Insight-Purple-2.png">
  <img src="https://khulnasoft/images/pr_insight/logo-light.png" alt="logo" width="330">

</picture>
<br/>

 [Installation Guide](https://pr-insight-docs.khulnasoft.com/installation/) |
[Usage Guide](https://pr-insight-docs.khulnasoft.com/usage-guide/) |
[Tools Guide](https://pr-insight-docs.khulnasoft.com/tools/) |
[Pr Merge](https://pr-insight-docs.khulnasoft.com/overview/pr_insight_pro/) 💎

PR-Insight aims to help efficiently review and handle pull requests, by providing AI feedback and suggestions
</div>

[![Static Badge](https://img.shields.io/badge/Chrome-Extension-violet)](https://chromewebstore.google.com/detail/pr-merge-ai-powered-cod/ephlnjeghhogofkifjloamocljapahnl)
[![Static Badge](https://img.shields.io/badge/Pro-App-blue)](https://github.com/apps/pr-merge-pro/)
[![Static Badge](https://img.shields.io/badge/OpenSource-App-red)](https://github.com/apps/pr-merge-pro-for-open-source/)
[![Discord](https://badgen.net/badge/icon/discord?icon=discord&label&color=purple)](https://discord.com/channels/1057273017547378788/1126104260430528613)
<a href="https://github.com/Khulnasoft/pr-insight/commits/main">
<img alt="GitHub" src="https://img.shields.io/github/last-commit/Khulnasoft/pr-insight/main?style=for-the-badge" height="20">
</a>
</div>

[//]: # (### [Documentation]&#40;https://pr-insight-docs.khulnasoft.com/&#41;)

[//]: # ()
[//]: # (- See the [Installation Guide]&#40;https://pr-insight-docs.khulnasoft.com/installation/&#41; for instructions on installing PR-Insight on different platforms.)

[//]: # ()
[//]: # (- See the [Usage Guide]&#40;https://pr-insight-docs.khulnasoft.com/usage-guide/&#41; for instructions on running PR-Insight tools via different interfaces, such as CLI, PR Comments, or by automatically triggering them when a new PR is opened.)

[//]: # ()
[//]: # (- See the [Tools Guide]&#40;https://pr-insight-docs.khulnasoft.com/tools/&#41; for a detailed description of the different tools, and the available configurations for each tool.)


## Table of Contents

- [News and Updates](#news-and-updates)
- [Overview](#overview)
- [Example results](#example-results)
- [Try it now](#try-it-now)
- [Pr Merge](https://pr-insight-docs.khulnasoft.com/overview/pr_insight_pro/)
- [How it works](#how-it-works)
- [Why use PR-Insight?](#why-use-pr-insight)

## News and Updates

## March 28, 2025
A new version, v0.28, was released. See release notes [here](https://github.com/khulnasoft/pr-insight/releases/tag/v0.28).

This version includes a new tool, [Help Docs](https://pr-insight-docs.khulnasoft.com/tools/help_docs/), which can answer free-text questions based on a documentation folder.

`/help_docs` is now being used to provide immediate automatic feedback to any user who [opens an issue](https://github.com/khulnasoft/pr-insight/issues/1608#issue-2897328825) on PR-Insight's open-source project

### Feb 28, 2025
A new version, v0.27, was released. See release notes [here](https://github.com/khulnasoft/pr-insight/releases/tag/v0.27).

### Feb 27, 2025
- Updated the default model to `o3-mini` for all tools. You can still use the `gpt-4o` as the default model by setting the `model` parameter in the configuration file.
- Important updates and bug fixes for Azure DevOps, see [here](https://github.com/khulnasoft/pr-insight/pull/1583)
- Added support for adjusting the [response language](https://pr-insight-docs.khulnasoft.com/usage-guide/additional_configurations/#language-settings) of the PR-Insight tools.


### December 30, 2024

Following feedback from the community, we have addressed two vulnerabilities identified in the open-source PR-Insight project. The [fixes](https://github.com/khulnasoft/pr-insight/pull/1425) are now included in the newly released version (v0.26), available as of today.


## Overview
<div style="text-align:left;">

Supported commands per platform:

|       |                                                                                                         | GitHub             | GitLab             | Bitbucket | Azure DevOps |
|-------|---------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:---------:|:------------:|
| TOOLS | [Review](https://pr-insight-docs.khulnasoft.com/tools/review/)                                                 | ✅ | ✅ |     ✅     |      ✅       |
|       | [Describe](https://pr-insight-docs.khulnasoft.com/tools/describe/)                                             | ✅ | ✅ |     ✅     |      ✅       |
|       | [Improve](https://pr-insight-docs.khulnasoft.com/tools/improve/)                                               | ✅ | ✅ |     ✅     |      ✅       |
|       | [Ask](https://pr-insight-docs.khulnasoft.com/tools/ask/)                                                       | ✅ | ✅ |     ✅     |      ✅       |
|       | ⮑ [Ask on code lines](https://pr-insight-docs.khulnasoft.com/tools/ask/#ask-lines)                             | ✅ | ✅ |           |              |
|       | [Update CHANGELOG](https://pr-insight-docs.khulnasoft.com/tools/update_changelog/)                             | ✅ | ✅ |     ✅     |      ✅       |
|       | [Help Docs](https://pr-insight-docs.khulnasoft.com/tools/help_docs/?h=auto#auto-approval)                      |   ✅    |   ✅    |   ✅        |            |
|       | [Ticket Context](https://pr-insight-docs.khulnasoft.com/core-abilities/fetching_ticket_context/) 💎            | ✅ | ✅ |     ✅     |   |
|       | [Utilizing Best Practices](https://pr-insight-docs.khulnasoft.com/tools/improve/#best-practices) 💎            | ✅ | ✅ |     ✅     |   |
|       | [PR Chat](https://pr-insight-docs.khulnasoft.com/chrome-extension/features/#pr-chat) 💎                        | ✅ |  |           |   |
|       | [Suggestion Tracking](https://pr-insight-docs.khulnasoft.com/tools/improve/#suggestion-tracking) 💎            | ✅ | ✅ |           |   |
|       | [CI Feedback](https://pr-insight-docs.khulnasoft.com/tools/ci_feedback/) 💎                                    | ✅ |                    |           |              |
|       | [PR Documentation](https://pr-insight-docs.khulnasoft.com/tools/documentation/) 💎                             | ✅ | ✅ |           |              |
|       | [Custom Labels](https://pr-insight-docs.khulnasoft.com/tools/custom_labels/) 💎                                | ✅ | ✅ |           |              |
|       | [Analyze](https://pr-insight-docs.khulnasoft.com/tools/analyze/) 💎                                            | ✅ | ✅ |           |              |
|       | [Similar Code](https://pr-insight-docs.khulnasoft.com/tools/similar_code/) 💎                                  | ✅ |                    |           |              |
|       | [Custom Prompt](https://pr-insight-docs.khulnasoft.com/tools/custom_prompt/) 💎                                | ✅ | ✅ |     ✅     |              |
|       | [Test](https://pr-insight-docs.khulnasoft.com/tools/test/) 💎                                                  | ✅ | ✅ |           |              |
|       | [Implement](https://pr-insight-docs.khulnasoft.com/tools/implement/) 💎                                        | ✅ | ✅ |     ✅     |              |
|       | [Auto-Approve](https://pr-insight-docs.khulnasoft.com/tools/improve/?h=auto#auto-approval) 💎                  |   ✅    |   ✅    |   ✅        |            |
|       |                                                                                                         |                    |                    |           |              |
| USAGE | [CLI](https://pr-insight-docs.khulnasoft.com/usage-guide/automations_and_usage/#local-repo-cli)                | ✅ | ✅ |     ✅     |      ✅       |
|       | [App / webhook](https://pr-insight-docs.khulnasoft.com/usage-guide/automations_and_usage/#github-app)          | ✅ | ✅ |     ✅     |      ✅       |
|       | [Tagging bot](https://github.com/Khulnasoft/pr-insight#try-it-now)                                         | ✅ |                    |           |              |
|       | [Actions](https://pr-insight-docs.khulnasoft.com/installation/github/#run-as-a-github-action)                  | ✅ |✅|     ✅     |✅|
|       |                                                                                                         |                    |                    |           |              |
| CORE  | [PR compression](https://pr-insight-docs.khulnasoft.com/core-abilities/compression_strategy/)                  | ✅ | ✅ |     ✅     |      ✅       |
|       | Adaptive and token-aware file patch fitting                                                             | ✅ | ✅ |     ✅     |      ✅       |
|       | [Multiple models support](https://pr-insight-docs.khulnasoft.com/usage-guide/changing_a_model/)                | ✅ | ✅ |     ✅     |      ✅       |
|       | [Local and global metadata](https://pr-insight-docs.khulnasoft.com/core-abilities/metadata/)                   | ✅ | ✅ |     ✅     | ✅             |
|       | [Dynamic context](https://pr-insight-docs.khulnasoft.com/core-abilities/dynamic_context/)                      | ✅ | ✅ |     ✅     | ✅             |
|       | [Self reflection](https://pr-insight-docs.khulnasoft.com/core-abilities/self_reflection/)                      | ✅ | ✅ |     ✅     | ✅             |
|       | [Static code analysis](https://pr-insight-docs.khulnasoft.com/core-abilities/static_code_analysis/) 💎         | ✅ | ✅ |           |              |
|       | [Global and wiki configurations](https://pr-insight-docs.khulnasoft.com/usage-guide/configuration_options/) 💎 | ✅ | ✅ |     ✅     |              |
|       | [PR interactive actions](https://www.khulnasoft.com/images/pr_insight/pr-actions.mp4) 💎                         | ✅ |        ✅           |           |              |
|       | [Impact Evaluation](https://pr-insight-docs.khulnasoft.com/core-abilities/impact_evaluation/) 💎               | ✅ | ✅ |           |   |
- 💎 means this feature is available only in [Pr-Merge](https://www.khulnasoft.com/pricing/)

[//]: # (- Support for additional git providers is described in [here]&#40;./docs/Full_environments.md&#41;)
___

‣ **Auto Description ([`/describe`](https://pr-insight-docs.khulnasoft.com/tools/describe/))**: Automatically generating PR description - title, type, summary, code walkthrough and labels.
\
‣ **Auto Review ([`/review`](https://pr-insight-docs.khulnasoft.com/tools/review/))**: Adjustable feedback about the PR, possible issues, security concerns, review effort and more.
\
‣ **Code Suggestions ([`/improve`](https://pr-insight-docs.khulnasoft.com/tools/improve/))**: Code suggestions for improving the PR.
\
‣ **Question Answering ([`/ask ...`](https://pr-insight-docs.khulnasoft.com/tools/ask/))**: Answering free-text questions about the PR.
\
‣ **Update Changelog ([`/update_changelog`](https://pr-insight-docs.khulnasoft.com/tools/update_changelog/))**: Automatically updating the CHANGELOG.md file with the PR changes.
\
‣ **Help Docs ([`/help_docs`](https://pr-insight-docs.khulnasoft.com/tools/help_docs/))**: Answers a question on any repository by utilizing given documentation.
\
‣ **Add Documentation 💎  ([`/add_docs`](https://pr-insight-docs.khulnasoft.com/tools/documentation/))**: Generates documentation to methods/functions/classes that changed in the PR.
\
‣ **Generate Custom Labels 💎 ([`/generate_labels`](https://pr-insight-docs.khulnasoft.com/tools/custom_labels/))**: Generates custom labels for the PR, based on specific guidelines defined by the user.
\
‣ **Analyze 💎 ([`/analyze`](https://pr-insight-docs.khulnasoft.com/tools/analyze/))**: Identify code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component.
\
‣ **Test 💎 ([`/test`](https://pr-insight-docs.khulnasoft.com/tools/test/))**: Generate tests for a selected component, based on the PR code changes.
\
‣ **Custom Prompt 💎 ([`/custom_prompt`](https://pr-insight-docs.khulnasoft.com/tools/custom_prompt/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
\
‣ **Generate Tests 💎 ([`/test component_name`](https://pr-insight-docs.khulnasoft.com/tools/test/))**: Generates unit tests for a selected component, based on the PR code changes.
\
‣ **CI Feedback 💎 ([`/checks ci_job`](https://pr-insight-docs.khulnasoft.com/tools/ci_feedback/))**: Automatically generates feedback and analysis for a failed CI job.
\
‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-insight-docs.khulnasoft.com/tools/similar_code/))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
\
‣ **Implement 💎 ([`/implement`](https://pr-insight-docs.khulnasoft.com/tools/implement/))**: Generates implementation code from review suggestions.
___

## Example results
</div>
<h4><a href="https://github.com/Khulnasoft/pr-insight/pull/530">/describe</a></h4>
<div align="center">
<p float="center">
<img src="https://www.khulnasoft/images/pr_insight/describe_new_short_main.png" width="512">
</p>
</div>
<hr>

<h4><a href="https://github.com/Khulnasoft/pr-insight/pull/732#issuecomment-1975099151">/review</a></h4>
<div align="center">
<p float="center">
<kbd>
<img src="https://www.khulnasoft/images/pr_insight/review_new_short_main.png" width="512">
</kbd>
</p>
</div>
<hr>

<h4><a href="https://github.com/Khulnasoft/pr-insight/pull/732#issuecomment-1975099159">/improve</a></h4>
<div align="center">
<p float="center">
<kbd>
<img src="https://www.khulnasoft/images/pr_insight/improve_new_short_main.png" width="512">
</kbd>
</p>
</div>


<div align="left">


</div>
<hr>


## Try it now

Try the Claude Sonnet powered PR-Insight instantly on _your public GitHub repository_. Just mention `@KhulnaSoft-Agent` and add the desired command in any PR comment. The agent will generate a response based on your command.
For example, add a comment to any pull request with the following text:
```
@KhulnaSoft-Agent /review
```
and the agent will respond with a review of your PR.

Note that this is a promotional bot, suitable only for initial experimentation.
It does not have 'edit' access to your repo, for example, so it cannot update the PR description or add labels (`@KhulnaSoft-Agent /describe` will publish PR description as a comment). In addition, the bot cannot be used on private repositories, as it does not have access to the files there.


---


## Pr Merge 💎
[Pr Merge](https://www.khulnasoft.com/pricing/) is a hosted version of PR-Insight, provided by Khulnasoft. It is available for a monthly fee, and provides the following benefits:
1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the Pr Merge app to your GitHub\GitLab\BitBucket repo.
2. **Improved privacy** - No data will be stored or used to train models. Pr Merge will employ zero data retention, and will use an OpenAI account with zero data retention.
3. **Improved support** - Pr Merge users will receive priority support, and will be able to request new features and capabilities.
4. **Extra features** -In addition to the benefits listed above, Pr Merge will emphasize more customization, and the usage of static code analysis, in addition to LLM logic, to improve results.
See [here](https://pr-insight-docs.khulnasoft.com/overview/pr_insight_pro/) for a list of features available in Pr Merge.



## How it works

The following diagram illustrates PR-Insight tools and their flow:

![PR-Insight Tools](https://www.khulnasoft.com/images/pr_insight/diagram-v0.9.png)

Check out the [PR Compression strategy](https://pr-insight-docs.khulnasoft.com/core-abilities/#pr-compression-strategy) page for more details on how we convert a code diff to a manageable LLM prompt

## Why use PR-Insight?

A reasonable question that can be asked is: `"Why use PR-Insight? What makes it stand out from existing tools?"`

Here are some advantages of PR-Insight:

- We emphasize **real-life practical usage**. Each tool (review, improve, ask, ...) has a single LLM call, no more. We feel that this is critical for realistic team usage - obtaining an answer quickly (~30 seconds) and affordably.
- Our [PR Compression strategy](https://pr-insight-docs.khulnasoft.com/core-abilities/#pr-compression-strategy)  is a core ability that enables to effectively tackle both short and long PRs.
- Our JSON prompting strategy enables to have **modular, customizable tools**. For example, the '/review' tool categories can be controlled via the [configuration](pr_insight/settings/configuration.toml) file. Adding additional categories is easy and accessible.
- We support **multiple git providers** (GitHub, Gitlab, Bitbucket), **multiple ways** to use the tool (CLI, GitHub Action, GitHub App, Docker, ...), and **multiple models** (GPT, Claude, Deepseek, ...)


## Data privacy

### Self-hosted PR-Insight

- If you host PR-Insight with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
https://openai.com/enterprise-privacy

### Khulnasoft-hosted Pr Merge 💎

- When using Pr Merge 💎, hosted by Khulnasoft, we will not store any of your data, nor will we use it for training. You will also benefit from an OpenAI account with zero data retention.

- For certain clients, Khulnasoft-hosted Pr Merge will use Khulnasoft’s proprietary models — if this is the case, you will be notified.

- No passive collection of Code and Pull Requests’ data — Pr Merge will be active only when you invoke it, and it will then extract and analyze only data relevant to the executed command and queried pull request.

### Pr Merge Chrome extension

- The [Pr Merge Chrome extension](https://chromewebstore.google.com/detail/pr-merge-ai-powered-cod/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the visual appearance of a GitHub PR screen. It does not transmit any user's repo or pull request code. Code is only sent for processing when a user submits a GitHub comment that activates a PR-Insight tool, in accordance with the standard privacy policy of Pr-Merge.

## Links

- Discord community: https://discord.gg/kG35uSHDBc
- Khulnasoftsite: https://www.khulnasoft.com/
- Blog: https://www.khulnasoft.com/blog/
- Troubleshooting: https://www.khulnasoft.com/blog/technical-faq-and-troubleshooting/
- Support: support@khulnasoft.com
