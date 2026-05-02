# Teacher's Guide: Python for Data Science

This guide outlines the pedagogical framework for managing this 16-week curriculum.

## Teaching Philosophy: Active Mentorship
This course utilizes a **flipped-classroom model**. The goal is to maximize one-on-one interaction time by shifting content delivery to pre-session materials.

- **Pre-session**: Ensure the student has reviewed the weekly `Explanation.md` and attempted the corresponding `ipynb` notebook.
- **Session Focus**: Use meeting time to review Pull Requests, debug issues, discuss architectural choices, and provide guidance on the "Practice" section (Exercism/Kaggle).

## Workflow & Assessment
1. **GitHub Classroom**: Use this to distribute materials and collect submissions.
2. **Code Review**: Treat student submissions as production code. Review them via Pull Requests, focusing on:
   - **Pythonic Idioms**: Are they using comprehensions, generators, and decorators appropriately?
   - **Vectorization**: Are they avoiding unnecessary loops in NumPy/Pandas?
   - **Best Practices**: Is the code modular, tested (`pytest`), and well-documented?
3. **Capstone Integration**: Use the Streamlit template in `capstone_template/` as the starting point for their final project to ensure they get early exposure to deployment.

## Technical Infrastructure
- **Quarto**: Use `quarto preview` to build and review course materials locally.
- **Git**: Ensure the student adheres to disciplined version control.
