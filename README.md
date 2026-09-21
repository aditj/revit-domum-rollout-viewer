# DOMUM reconstruction evidence viewer

A static Collinear viewer for the image-only Revit reconstruction benchmark. Hosted on Render.

Includes 303 captured Sol frames with recorded UI actions, six final reference/candidate comparisons, seven 2D input sheets, the task instruction, rubric reasoning, and the saved Sol project. Astra's interrupted score is shown with an explicit missing-artifact notice; its visuals and criterion breakdown are not fabricated.

No backend, API credentials, raw session logs, system prompts or analytics. Data is packaged from a fixed run snapshot. Scores are rubric scores, not geometric accuracy percentages.

Run locally: `uv run python -m http.server 3092 --directory .`.
Render: Static Site, branch `main`, build command `echo static`, publish directory `.`.

Source runs: Astra `2026-09-21T1843-adit-aa2b`; Sol `2026-09-21T1843-adit-c624`. Asset packaging script lives in the Nexus experiment at `experiments/revit-domum-reconstruction/site-source/package.py`.
