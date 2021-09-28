+++
title = "Harsh's Internship Presentation"
outputs = ["Reveal"]
+++

# Re-Engineering CI/CD pipelines for Scipy

Harsh Mishra

{{< social >}}
{{< talk-link qs-intern-talk >}}


{{< figure src="images/labs.jpg" height="60px" >}}

---

# Agenda

- {{< frag c="Introduction to the Project" >}}
- {{< frag c="Project implementation" >}}
- {{< frag c="Learnings out of the Project" >}}
- {{< frag c="Future plan for the project" >}}
- {{< frag c="Acknowledgement" >}}
- {{< frag c="Q&A" >}}

---

# About the project!

- {{< frag c="Re-engineer the CI pipelines for Scipy to be compatible with Meson." >}}
- {{< frag c="Enable local debugging of CI Actions using Act." >}}
- {{< frag c="Implement GitHub Actions for building and testing on macOS." >}}
- {{< frag c="Plan the CI matrix for the upcoming Scipy build setup using Meson." >}}
- {{< frag c="Implement CI benchmarking using GitHub Actions to be compatible with ASV" >}}

---

# Project implementation: [PR#57](https://github.com/rgommers/scipy/pull/57)

- {{< frag c="Configured `act` to run the GitHub Action workflows locally." >}}
- {{< frag c="Refactored the `meson.build` to generate `__config__.py` and `version.py` dynamically." >}}
- {{< frag c="Wrote the documentation on usage of `act` with GitHub Actions." >}}

---

# Project implementation: [PR#59](https://github.com/rgommers/scipy/pull/63)

- {{< frag c="Implemented build caching for Meson to restore compiler targets for faster builds." >}}
- {{< frag c="Reduced the build time by 70% on the GitHub Actions CI (takes ~3 minutes for a build)" >}}
- {{< frag c="Integrated timestamp-based caching to cache and restore the latest compiler targets." >}}

---

# Project implementation: [PR#65](https://github.com/rgommers/scipy/pull/65)

- {{< frag c="Implemented the Scipy build and test CI action for macOS using GitHub Actions." >}}
- {{< frag c="Reduced the build time by 30% on the GitHub Actions CI using ccache compiler caching." >}}
- {{< frag c="Integrated conda caching and Mamba for faster installs and build time." >}}

---

# Project implementation: [PR#67](https://github.com/rgommers/scipy/pull/67)

- {{< frag c="Implemented the automated benchmarking on GitHub Actions CI using ASV." >}}
- {{< frag c="Automatically builds Scipy and runs a benchmark action to compare the base commit with the PR commit." >}}
- {{< frag c="Uploads the ASV results, generated HTML files and the benchmark logs to be verified on demand." >}}

---

# Miscellaneous

- Enhanced the Scipy Issue templates to utilize GitHub Issue Forms [[PR#14493](https://github.com/scipy/scipy/pull/14493)]
- Refactored the Scipy Issue templates to improve the user experience [[PR#14669](https://github.com/scipy/scipy/pull/14669)]
- Strategized the CI matrix for Scipy's Meson build system, available here on the [Sheet-3](https://docs.google.com/spreadsheets/d/1YAiJsaHBIUwefn2KMQv11uH1EeIKfY4cU1KfoLbl6VY/edit?usp=sharing).

---

# Learnings out of the Project

- {{< frag c="Learnt about Meson build system and custom targets." >}}
- {{< frag c="Increased my familiarity with GitHub Actions and CI toolings." >}}
- {{< frag c="Understood caching and benchmarking through working on an actual project." >}}
- {{< frag c="Real-time collaboration and communication with my mentor and stakeholders." >}}

---

# Future plan for the project

- {{< frag c="Start working on the CI matrix and remove CI-deadweight." >}}
- {{< frag c="Build and test the new Meson build on various architectures through GitHub Actions." >}}
- {{< frag c="Implement GHA release action for automating the release of source archives." >}}

---

# Acknowledgement

- Thanks to my mentor, [John Lee](https://github.com/leej3) for providing the necessary guidance and feedback on every step.
- Thanks [Ralf Gommers](https://github.com/rgommers/) for helping with feedback, suggestions and reviews.
- Thanks [Anirudh Dagar](https://github.com/AnirudhDagar) for providing necessary motivation and reviews.
- Thanks [Jaime Rodríguez-Guerra](https://github.com/jaimergp) for helping with CI benchmarking and other stuff.

---

# Thanks!

{{% grid middle %}}

{{< g 1 >}}
{{< figure src="images/quansight_logo_white.png" height="280px" >}}


{{< /g >}}

{{< g 1 >}}

Harsh Mishra
{{< social >}}
{{< talk-link qs-intern-talk >}}

{{< /g >}}

{{% /grid %}}
