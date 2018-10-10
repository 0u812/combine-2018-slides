##  Future directions

<ul>
  <li> SemGen integration (collab. with John Gennari) </li>
  <li> Cloud-based (e.g. AWS) support for compute-intensive tasks (active project) </li>
  <li class="fragment"> Upgrade to [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/) </li>
  <li class="fragment"> Unified syntax for inline OMEX
    <ul>
      <li> SBML, CellML, SED-ML </li>
    </ul>
  </li>
  <li class="fragment"> Support for other Python-based simulators?
    <ul>
      <li> PySCeS, PySB, COPASI </li>
    </ul>
  </li>
  <li class="fragment"> Scripting &amp; SED-ML
    <ul>
      <li> Want generic capability (like SESSL) </li>
    </ul>
  </li>
</ul>

note:
    ∙ Our next target feature is to provide a Python solution for compute-intensive tasks, such as
    calibrating models with nonlinear optimization. This is a feature we're actively working on,
    and our plan is to provide a solution that will allow people to set up their own optimization
    problems with their own custom objective functions and run them in the AWS or Google cloud.
    That's our immediate goal.
    <br/>
    ∙ As part of a more long-term effort, I think this approach would really benefit from having
    a syntax designed to support embedding SBML, CellML, and SED-ML in the same parser.
    Currently, Tellurium breaks up the omex cell into chunks and sends them to different parsers depending
    on whether the chunk represents SBML or SED-ML, but that's an error-prone process in not very scalable.
    The upshot is that it allows us to prototype ideas and use cases and see what that kind of unified
    syntax would look like, but I think eventually we're going to get tripped up unless we can
    unify this syntax.
    <br/>
    ∙ Jupyter lab is an evolution of the Jupyter notebook which is a little more feature complete,
    and is more suitable to large projects, and so we would like to update our notebook viewer to take
    advantage of those UI improvements.
    <br/>
    ∙ At least for my own future plans, I would like to provide convenience wrappers for other Python-based simulators.
    Currently, users can of course export SBML models from Antimony and import them into other simulators,
    but this is a manual process and it would be much better to have the functionality to do that automatically.
    Roadrunner and Antimony are designed for interoperability, but they will probably
    never cover all SBML packages, so there will always be a need for users to be able to use
    third-part simulators, e.g. PySB for rule-based modeling.
    <br/>
    SED-ML generics wide open. From a user perspective, you would ideally
    want to be able to support all the various things people do with their models.
    SESSL has a great solution to this, but doesn'h have the advantages of a standard representation.
