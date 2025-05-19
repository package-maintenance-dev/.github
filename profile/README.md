### package-maintenance.dev
This project analyzes binary packages from sources like Maven Central and PyPI, linking them to their corresponding source repositories (e.g., on GitHub).
It calculates a set of activity-based metrics—using both binary and source data—to evaluate the maintenance state of each package.

These metrics can be used to manually assess a package or library in the [web app](https://package-maintenance.dev), or to automatically audit your project dependencies using tools like the [GitHub action](https://github.com/package-maintenance-dev/github-action).

Discussion & Feedback
This project is under active development, and your feedback is greatly appreciated.

Whether you’ve:

Spotted confusing scores
Found gaps in the index
Have ideas for new metrics
Please open a discussion or create an issue. 

See Examples
- [Poetry + Python example](https://github.com/package-maintenance-dev/github-action-poetry-example)
- [Gradle + Java example](https://github.com/package-maintenance-dev/github-action-gradle-example)
- [Maven + Java example](https://github.com/package-maintenance-dev/github-action-maven-example)
- [SBT + Scala example](https://github.com/package-maintenance-dev/github-action-sbt-example)
