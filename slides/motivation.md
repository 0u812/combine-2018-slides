

<div class="container">
  <div class="containercol">
    <ul>
      <li style="margin-bottom: 1.5em">
        COMBINE archives
      </li>
      <li class="fragment" style="margin-bottom: 1.5em">
        Exchangeability 👍
      </li>
      <li class="fragment" style="margin-bottom: 1.5em">
        Usability 👎
      </li>
      <li class="fragment" style="margin-bottom: 1.5em">
        Solution?
      </li>
    </ul>
  </div>
  <div class="containercol" style="flex-grow:1.5">
    <img src="resources/combine-archive-file-types-plain.svg" style="width:70%;height:auto"/>
  </div>
</div>

note:
    ∙ So in order to talk about this project, we need to talk about COMBINE archives. For those who don't know, COMBINE archives were designed to solve the problem of exchanging standards between software tools. In this COMBINE umbrella organization, we have many different types of standards such as SBML, CellML, SED-ML, and the files encoded in these standards can be interdependent. So, when you have interdependent files like this, it's very difficult to manually exchange the collection of files between software tools. Instead, you can package the files in a COMBINE archive, which is a single file that the user sees on their desktop, but inside it contains all pertinent standard files to reproduce the study.<br/>
    ∙ So, COMBINE archives solve the problem of exchangeability, but they create a problem of usability. In other words, given a COMBINE archive and all these diverse standards it contains, how do you display the information to the user and how to you allow them to edit the contents and re-export to a COMBINE archive?<br/>
    ∙ Our project was motivated by the problem of allowing the user to author, edit and export COMBINE archives.

