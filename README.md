# The Encyclopedia of Economic Principals: companion notebooks and skills

Companion material for *The Encyclopedia of Economic Principals* by Jason Karpeles. Each of the
book's 99 chapters has a Jupyter notebook that reproduces its worked examples and figures, and a
skill that an AI assistant can use to apply the chapter's principles to your own numbers.

Interactive version: https://karpeles.com/companions/economic-principles/
About the book: https://karpeles.com/publishing/the-encyclopedia-of-economic-principals

## What is here

- `notebooks/`: one notebook per chapter, already run, so the results show on GitHub. Each notebook is self-contained: every function it uses is written out in the notebook.
- `skills/`: a master skill for the book and one skill per chapter.
- `requirements.txt`: the Python packages the notebooks need.

## Run the notebooks

You need Python 3.11 or later.

    pip install numpy scipy matplotlib jupyterlab
    jupyter lab

(or `pip install -r requirements.txt`). Open any notebook in `notebooks/` and choose Run All.

## Use the skills

Each folder in `skills/` holds a `SKILL.md` file. To use one with Claude Code, copy the folder into `~/.claude/skills/` (or into your agent's skills folder):

    cp -r skills/economic-principles-guide ~/.claude/skills/
    cp -r skills/ep-ch033-oligopoly-cournot-bertrand-capacity-and-leadership ~/.claude/skills/

The [master skill](skills/economic-principles-guide/SKILL.md) routes a question to the right chapter and principle. Each chapter skill gives the chapter's equations, the steps to apply them to your own inputs with the book's example in parentheses, and points to that chapter's notebook.

## Copyright

Copyright Jason Karpeles. All rights reserved.
