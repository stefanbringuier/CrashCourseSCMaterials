[🎥 PRESENTATION](https://stefanbringuier.github.io/CrashCourseSCMaterials)

## Presentation: Crash Course in Materials Science of Superconductors
These are note for anyone who is interested in quickly familiarizing themselves with superconductors from a materials science perspective. A good portion of the notes are based on the references provided at the end.

The presentation can be viewed on [https://stefanbringuier.github.io/CrashCourseSCMaterials](https://stefanbringuier.github.io/CrashCourseSCMaterials) and PDF report-style version can be accessed [here](https://stefanbringuier.github.io/CrashCourseSCMaterials/presentation_reportformat.pdf). This presentation uses  the [quarto](quarto.org) package to build a [revealjs](revealjs.com) presentation. 


## Setup to render/modify presentation
The document preparation is carried out in [VSCode](code.visualstudio.com) using the [quarto](quarto.org) extension. The executed code blocks in this presentation are done in [python](python.org) or [Julia](julialang.org).

1. Install [Quarto](https://quarto.org/docs/get-started/)
2. Install Julia
3. Clone the repo
4. Instantiate the Julia project:
    ```shell
    cd CrashCourseSCMaterials
    julia --project=@.
    ```
    ```julia
    julia> ]
    (BayesianOptNotes) pkg> instantiate
    julia> using IJulia
    julia> notebook()
    julia> `press CTRL+C`
    julia> using Conda
    julia> Conda.add("jupyter-cache")
    julia> exit()
    ```
4. Render document/project :
    ```shell
    quarto render .
    ```

Peforming these steps will produce a [revealjs](revealjs.com) in the [output](output) folder along with a [report style pdf](output/presentation_reportformat.pdf). 