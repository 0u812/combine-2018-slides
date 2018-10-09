Tellurium is an umbrella package that consists of:

* `libroadrunner`: SBML simulator
* `antimony`/`phrasedml`: Read/write COMBINE standards
* Many others

Key feature: Make standards accessible

note:
    ∙ I mentioned that Tellurium can be used in a literal notebook environment based on the Python programming language. The Python code that makes Tellurium work is also available independently as an umbrella package designed to contain everything you need to author and simulate models in Combine standards. I also wanted to provide a more detailed breakdown of the components for the more technical users here.
    <br/>
    ∙ Tellurium contains an SBML simulator called libroadrunner, and it also contains parsers for SBML and SED-ML that allow you to edit those standards in this human-readable form (credit Lucian). Tellurium itself abstracts these components so you don't have to be an expert in them or even know they're there.
    <br/>
    ∙ Tellurium's key feature is that it makes standards accessible to researchers outside of standards development who may not be familiar with the standards or want to waste valuable resources understanding the details of how the standards are encoded. We basically want to give people an alternative to Matlab which they can use to prepare publication-quality ODE and stochastic models. The notebook format really helps ease the transition into standards, and we have provided a lot of examples to cover the most common use cases in modeling. You'll see some examples in this talk, and the rest are bundled with the notebook viewer itself and the online documentation.
    <br/>
    ∙ When we first tried to publish this years ago, one question we got a lot from reviewers is why have an umbrella package at all? Well, the short answer is that we were trying to get people to move away from Matlab, and we were focused on having the most integrated experience possible. However, since that time we have also tried to modularize the design a bit, and as a consequence you can now install all these packages separately via pip or you can just download the Tellurium Notebook viewer and have all the packages included for you. So, all of these packages including tellurium itself are installable via pip, you're not forced to use the notebook viewer to get them.
    <br/>
