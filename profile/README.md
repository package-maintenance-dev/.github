# 📦 package-maintenance.dev

This project searchs binary packages from sources like Maven Central and PyPI, and links them to their source repositories (e.g., on GitHub).
Based on binary and source repository activity it evaluates a number of metrics. Grades each metric (A–D) to help you assess package support status
Highlights unsupported or at-risk dependencies in your project
These insights are especially useful for dependency audits, security reviews, and ensuring long-term project health.

🚀 GitHub Action: Dependency Maintenance Report

The package-maintenance-dev/github-action allows you to run a package audit directly in your CI pipeline.

✅ Features
Works with GitHub’s Dependency Graph
Outputs a markdown report in the GitHub Actions job summary
Highlights unsupported packages based on configurable thresholds
Supports ignore lists and score customization
🛠 Example Usage
```
uses: package-maintenance-dev/github-action@v0.0.1
with:
  github-token: ${{ secrets.GITHUB_TOKEN }}
  packages-ignore: |
    pkg:pypi/django
  packages-scores-thresholds: "source.commit.frequency:B,binary.release.recency:A"
⚠️ Make sure the Dependency Graph is enabled in your repository for the action to work.
📊 Metrics Explained
```
Each package is scored and graded on:

Metric	Description
Release recency	How recent the latest release is (months)
Commits recency	How recent the last commit is (months)
Commits frequency	Average commits/month (last 100 commits)
Issues lifetime	Average issue resolution time (days)
Issues open %	% of open issues (last 100)
PR lifetime	Average PR resolution time (days)
PR open %	% of open pull requests (last 100)
Each value is graded:

🟢 A – Top 10% of the index
🟡 B – Top 75%
🟠 C – Bottom 75%
🔴 D – Archived or unmaintained
📚 Learn More

🖥️ Web Application
⚙️ GitHub Action Documentation
📦 API & Score Index Docs
🤝 Contributing

We welcome contributions! Feel free to open issues or submit pull requests.

Let me know if you'd like a more minimal, technical, or marketing-oriented version.

You said:
Replace contributing section discussion section - to motivate users to provide feedaback
ChatGPT said:
You're giving feedback on a new version of ChatGPT.
Which response do you prefer? Responses may take a moment to load.
ChatGPT
Response 1
Here’s the updated version of the "Discussion" section to replace the "Contributing" section, with a focus on encouraging users to provide feedback:

💬 Discussion & Feedback

We’re actively improving package-maintenance.dev, and your feedback is essential.

Have ideas for new features? Noticed inaccurate results? Want support for more ecosystems?
Please share your thoughts by opening a discussion or creating an issue.

Your input helps us make the tools more reliable and useful for everyone.

Let me know if you'd like to also include a short feedback form link or email.


I prefer this response
ChatGPT
Response 2
Here's the updated version of the README.md with the "Contributing" section replaced by a "Discussion & Feedback" section to encourage users to share feedback:

🧰 Package Maintenance

package-maintenance.dev helps you audit and monitor the health of your project dependencies across ecosystems like Maven and PyPI. It provides activity-based maintenance metrics based on both binary package metadata and corresponding source repositories (e.g., GitHub), helping you identify unsupported or poorly supported dependencies.

🔎 Visit https://package-maintenance.dev to explore the web application.
📦 What It Does

Analyzes binary packages from sources like Maven Central and PyPI
Links them to their source repositories (e.g., on GitHub)
Calculates metrics like:
Release recency
Source commit activity
Issue and PR maintenance
Grades each metric (A–D) to help you assess package support status
Highlights unsupported or at-risk dependencies in your project
These insights are especially useful for dependency audits, security reviews, and ensuring long-term project health.

🚀 GitHub Action: Dependency Maintenance Report

The package-maintenance-dev/github-action allows you to run a package audit directly in your CI pipeline.

✅ Features
Works with GitHub’s Dependency Graph
Outputs a markdown report in the GitHub Actions job summary
Highlights unsupported packages based on configurable thresholds
Supports ignore lists and score customization
🛠 Example Usage
uses: package-maintenance-dev/github-action@v0.0.1
with:
  github-token: ${{ secrets.GITHUB_TOKEN }}
  packages-ignore: |
    pkg:pypi/django
  packages-scores-thresholds: "source.commit.frequency:B,binary.release.recency:A"
⚠️ Make sure the Dependency Graph is enabled in your repository for the action to work.
📊 Metrics Explained

Each package is scored and graded on:

Metric	Description
Release recency	How recent the latest release is (months)
Commits recency	How recent the last commit is (months)
Commits frequency	Average commits/month (last 100 commits)
Issues lifetime	Average issue resolution time (days)
Issues open %	% of open issues (last 100)
PR lifetime	Average PR resolution time (days)
PR open %	% of open pull requests (last 100)
Each value is graded:

🟢 A – Top 10% of the index
🟡 B – Top 75%
🟠 C – Bottom 75%
🔴 D – Archived or unmaintained
💬 Discussion & Feedback

We’re building package-maintenance.dev to be as useful and insightful as possible—and your feedback matters.

Whether you’ve:

Spotted confusing scores
Found gaps in the index
Have ideas for new metrics
Want to share your use case or success story
👉 Please open a discussion or create an issue to let us know. We'd love to hear from you.

📚 Learn More

🖥️ Web Application
⚙️ GitHub Action Documentation
📦 API & Score Index Docs
