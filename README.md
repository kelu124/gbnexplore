
# Sustainable-City Use-Case Explorer

*Connecting PROBONO use cases with real-world projects through automated LLM discovery.*

This tool takes the 49 sustainable-city use cases defined in the **PROBONO** project and extends them with fresh, comparable examples from around the world.

Each use case is sent to **Perplexity AI**, which returns up to five similar initiatives. Those findings are stored, published on a GitHub Page, and positioned on the **ISO 37101** matrix (12 purposes × 6 enablers) for quick visual orientation.


## What the tool actually does

**1. Takes a PROBONO use case**
Each one comes with a description and a location context.

**2. Generates targeted search prompts**
The prompt is filled programmatically (e.g. `{Place}`, `{use_case}`), then sent to the Perplexity model.

**3. Collects 5 similar projects/initiatives**
No rewriting, no embellishment — just what the model finds.

**4. Stores the results**
Structured dataframe for later reuse, analysis, or re-processing.

**5. Publishes everything to a GitHub Page**
Each use case gets its own page showing:

* The original PROBONO description
* The five discovered similar projects
* The ISO 37101 position (matrix cell)

**6. Maps items on the ISO 37101 framework**
Every result is tagged to one of the **12 purposes** and one of the **6 enablers**, producing a 12×6 grid that acts as the project’s navigation layer.


## Why this exists

Cities, infrastructure teams, and sustainability groups often ask the same question:

*“Who else has done something like this, and where?”*

The PROBONO use-case catalogue is a strong starting point, but it becomes far more useful when connected to real examples.

This tool automates that connection.


## How the tool is organised

* `pbn37k` → library used for the ISO37101 mapping.

* `data/` → raw PROBONO use cases
* `output`  → stored search results
* `docs/` → GitHub Pages output (static HTML + generated content) 



## Running it

See the notebook in here.

## Outputs

* **Structured dataset** of 49 use cases × 5 examples
* **ISO 37101 matrix view** for each 
* **Search history** for reproducibility, as a dump
* **Reference list** of external projects and sources, through the links


# Acknowledgements

We gratefully acknowledge the funding support of the European Union 
Horizon 2020 research project PROBONO under grant agreement no. 
101037075. Thank you to the PROBONO team.

# License

## CC by NC ND 

* © 2025  Mott MacDonald
* This work is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0).  
* https://creativecommons.org/licenses/by-nc-nd/4.0/

## In short

You are free to:
* Share — copy and redistribute the material in any medium or format
* The licensor cannot revoke these freedoms as long as you follow the license terms.

Under the following terms:
* Attribution — You must give appropriate credit , provide a link to the license, and indicate if changes were made . You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
* NonCommercial — You may not use the material for commercial purposes .
* NoDerivatives — If you remix, transform, or build upon the material, you may not distribute the modified material.
* No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

Notices:
* You do not have to comply with the license for elements of the material in the public domain or where your use is permitted by an applicable exception or limitation .
* No warranties are given. The license may not give you all of the permissions necessary for your intended use. For example, other rights such as publicity, privacy, or moral rights may limit how you use the material.