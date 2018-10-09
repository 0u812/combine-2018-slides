| Standard Encoding | vs. | <div class="container"> <div class="verticalcenter" style="flex-grow:0.3"> <img src="resources/matlab.png" style="width:60%;height:auto"/> </div> <div class="containercol"> Ad-hoc (e.g. with Matlab) </div> </div> |
|---|---|---|
<!--| <span class="fragment" data-fragment-index="1">∙ Composable</span> | <span class="fragment" data-fragment-index="1">∙ Not composable</span> |
| <span class="fragment" data-fragment-index="2">∙ Future-proof</span> | <span class="fragment" data-fragment-index="2">∙ Not future-proof</span> |-->

<div class="container">
<div class="verticalcenter fragment" data-fragment-index="1"> <img src="resources/insulin-egfr.png" style="width:70%;height:auto"/> <br/> ∙ [Composable](http://msb.embopress.org/content/5/1/256) </div>
<div class="verticalcenter fragment" data-fragment-index="2"> <img src="resources/noble.jpg" style="width:70%;height:auto"/> <br/> ∙ Future-proof </div>
<div class="verticalcenter fragment" data-fragment-index="3"> <img src="resources/microchip.jpg" style="width:70%;height:auto"/> <br/> ∙ Performant </div>
</div>

<span class="fragment fade-in" data-fragment-index="2" style="font-size:0.75em">
<span class="fragment fade-out" data-fragment-index="4"> Noble, Denis (1960). ["Cardiac action and pacemaker potentials based on the Hodgkin-Huxley equations"](https://doi.org/10.1038%2F188495b0). *Nature*. **188** (4749): 495–7.</span></span>

<span class="fragment fade-in" style="position:relative;top:-120px;font-size:2em;text-decoration: underline;color:#ff2c2d" data-fragment-index="4"> **BUT** </span>

note:
    ∙ We develop tools to support this kind of model. (standards)
    There are a number of reasons to use a standard encoding instead of
    coming up with ad-hoc Matlab code to run your model. Some reasons include:
    <br/>
    ∙ You can re-use smaller models by including them in bigger models, that's composability. For example, if you have a model of the EGFR pathway and the insulin
    signaling pathway, you can actually combine these into a single larger model. This works because the standard actually preserves the individual processes and intermediates in each submodel. You may have to redefine the common intermediates, but it's certainly an improvement over the massive amount of reengineering you would have to do for the Matlab case.
    ∙ You can future-proof your models and preserve them for all time. This is Denis Noble, who created a model of pacemaker potentials in the heart in 1960 based on the Hodgkin-Huxley equations, and his models have been preserved for all posterity in a standard encoding. They can be opened, edited, and simulated using modern software. In this case, the model obviously pre-dated the standard, but once encoded a model becomes future-proof.
    ∙ And finally, the model encoding is separate from the software used to simulate it. This is important because your model can take advantage of future standards-supporting simulators, simply by being encoded in the standard. It's a free speedup, and as we start building whole-tissue models that is going to be more and more important. There's even special-purpose hardware for simulating standard-encoded models. If you're familiar with Bitcoin mining, you know that special-purpose hardware vastly outperforms CPUs, and the same is typically true for any other domain, including kinetic models.
    ∙ All of these points are essential for multiscale modeling, and our ability to make progress with our modeling art depends on them.
    ∙ BUT for all the advantages of the standard-encoded approach, there is a major disadvantage: it's difficult! It's difficult because the standards are highly technical. Understanding the standards can be even more challenging than building your model, whereas the Matlab is easy, and this fact alone usually determines which fork to take here.
