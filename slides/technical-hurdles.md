<!-- Credits: -->
<!-- https://en.wikipedia.org/wiki/XML -->
<!-- https://commons.wikimedia.org/wiki/File:Crystal128-pdf.svg -->
<div style="text-align: center">
<div style="position:relative;display:inline-block">
<img style="position:relative" src="resources/xml.svg" style="width:100%;height:auto;transform: scale(1.5,1.5)"/>
<img style="position:absolute;top:0px;left:0px;transform: rotate(20deg);" class="fragment" src="resources/sbml-levels-versions.svg"/>
<img style="position:absolute;top:0px;left:0px;transform: rotate(-15deg);" class="fragment" src="resources/sbml-uml.png"/>
<img style="position:absolute;top:0px;left:0px;transform: rotate(10deg);" class="fragment" src="resources/whoa-mind.gif"/>
</div>
</div>

<span class="fragment">Can we get rid of this complexity?</span>

note:
    Say you wanted to encode your model in a standard format. You could start by looking
    up the Systems Biology Markup Language (SBML), which is one of the standards. <br/>
    ∙ First, you find out that SBML is written in something called XML, which
    you may know about if you're a web or Rosetta developer, but otherwise will have to
    learn. <br/>
    ∙ Next, you try to look the SBML spec and you notice there's different versions along with these things called levels, there's three different specs, so it's starting to look like supporting the standard is going to be a really long and burdensome detour in your work. <br/>
    ∙ Finally, each spec contains over 150 pages of this stuff called UML diagrams, and a ton of technical details that don't have their use cases explained and most of which you probably don't even need, but you have to read all of it to make sure. <br/>
    ∙ So, no wonder people still publish in Matlab! If you're a modeler, you want to focus on understanding your system, you don't want to focus on reading the standard spec and supporting the standard. All this complexity in the standards is a bad thing, because it takes resources away from people doing the scientific work of building the models and forces them to spend that effort understanding the standards instead. <br/>
    ∙ So, the question is: can we get rid of this complexity and still allow modelers to use standards? And the answer is yes.