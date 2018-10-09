

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
    This project was born out of the need to solve a problem related to COMBINE archives. For those who don't know COMBINE archives are designed to solve the problem of exchanging files when you have multiple standards. In COMBINE, there's not just one filetype, there are many types, like SBML, CellML, SED-ML, and moreover they're interdependent, so COMBINE archives are designed to packae all the interdependent parts together.
    <br/>
    ∙ COMBINE archives basically are containers for a bunch of standard types, and they solved the problem of exchangeability between different software tools, but they created a new problem: given a COMBINE archive, how do you display the information to the user? Do you break it up and group it by the type of standard?
